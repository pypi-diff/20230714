# Comparing `tmp/clearner-0.9.83.tar.gz` & `tmp/clearner-0.9.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearner-0.9.83.tar", last modified: Sat Jun 17 03:00:04 2023, max compression
+gzip compressed data, was "clearner-0.9.84.tar", last modified: Wed Jul 12 02:50:18 2023, max compression
```

## Comparing `clearner-0.9.83.tar` & `clearner-0.9.84.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.748425 clearner-0.9.83/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.83/LICENSE
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-06-17 03:00:04.748425 clearner-0.9.83/PKG-INFO
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.728425 clearner-0.9.83/clearner.egg-info/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-06-17 03:00:04.000000 clearner-0.9.83/clearner.egg-info/PKG-INFO
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-06-17 03:00:04.000000 clearner-0.9.83/clearner.egg-info/SOURCES.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-06-17 03:00:04.000000 clearner-0.9.83/clearner.egg-info/dependency_links.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-06-17 03:00:04.000000 clearner-0.9.83/clearner.egg-info/entry_points.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-06-17 03:00:04.000000 clearner-0.9.83/clearner.egg-info/requires.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-06-17 03:00:04.000000 clearner-0.9.83/clearner.egg-info/top_level.txt
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.728425 clearner-0.9.83/learner/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/__init__.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.732425 clearner-0.9.83/learner/analysis/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/analysis/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/analysis/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/analysis/plot.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26790 2023-06-16 23:02:02.000000 clearner-0.9.83/learner/analysis/shap.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.732425 clearner-0.9.83/learner/api_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/api_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/api_worker/google_drive.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.732425 clearner-0.9.83/learner/callback_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/callback_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/callback_manager/callback.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.732425 clearner-0.9.83/learner/combine/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/combine/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/combine/combining_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.732425 clearner-0.9.83/learner/communication/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/communication/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/communication/communication_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/communication/email_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.736425 clearner-0.9.83/learner/configuration/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/configuration/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17522 2023-06-16 22:27:29.000000 clearner-0.9.83/learner/configuration/analysis.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/column.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/combine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/communication.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/configuration.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/connection.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2023-06-16 23:56:39.000000 clearner-0.9.83/learner/configuration/data.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/defaults.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.83/learner/configuration/feature_engineering.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/model.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/configuration/outlier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/process.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/configuration/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/sample.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/segmenter.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/configuration/similarities.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8287 2023-06-02 02:15:58.000000 clearner-0.9.83/learner/configuration/supported_items.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/configuration/validation.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/configuration/workspace.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.740425 clearner-0.9.83/learner/data_worker/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/data_worker/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.83/learner/data_worker/data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/data_mover.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 02:21:33.000000 clearner-0.9.83/learner/data_worker/data_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13606 2023-06-02 02:15:58.000000 clearner-0.9.83/learner/data_worker/data_sampler.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/data_segmenters.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/data_set.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/deep_tabular_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/image_data_loader.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/image_data_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/data_worker/image_processor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    16872 2023-06-16 23:27:46.000000 clearner-0.9.83/learner/data_worker/output_handler.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.740425 clearner-0.9.83/learner/engines/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/engines/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/base_deep_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14832 2023-06-16 23:27:46.000000 clearner-0.9.83/learner/engines/base_standard_engine.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/deep_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/deep_regressor.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/engine_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/image_classifier.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/recommender.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14685 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/engines/standard_engines.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.740425 clearner-0.9.83/learner/feature_engineering/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/feature_engineering/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.83/learner/feature_engineering/feature_engineering.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.744425 clearner-0.9.83/learner/model_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/model_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/deep_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/deep_loop_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/deep_regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/extenders.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/image_classifiers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/layer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/loss_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/model_initializer.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/nn_utils.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/optimizer_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/prediction_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2023-05-19 05:22:49.000000 clearner-0.9.83/learner/model_manager/regressors.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/model_manager/scheduler_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/model_manager/scorers.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23613 2023-06-02 02:15:58.000000 clearner-0.9.83/learner/model_manager/scoring_manager.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2412 2023-06-02 02:15:58.000000 clearner-0.9.83/learner/model_manager/similarities.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.744425 clearner-0.9.83/learner/outlier_manager/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/outlier_manager/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/outlier_manager/outlier_manager.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.744425 clearner-0.9.83/learner/schema/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/schema/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/schema/credentials_schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/schema/logging.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/schema/meta_data.schema.json
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.83/learner/schema/schema.json
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.748425 clearner-0.9.83/learner/setup/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/setup/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/setup/logger.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-06-16 22:41:31.000000 clearner-0.9.83/learner/setup/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/setup/parser.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/setup/setup.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.748425 clearner-0.9.83/learner/utilities/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/utilities/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/utilities/exclude.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3905 2023-06-02 02:15:58.000000 clearner-0.9.83/learner/utilities/progress_bar.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/utilities/smtp.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1674 2023-06-16 21:44:22.000000 clearner-0.9.83/learner/utilities/templates.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/utilities/timer.py
-drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-06-17 03:00:04.748425 clearner-0.9.83/learner/validator/
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/validator/__init__.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/validator/column_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.83/learner/validator/data_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/validator/input_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/validator/model_validator.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.83/learner/validator/output_validator.py
--rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.83/main.py
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-06-02 02:15:58.000000 clearner-0.9.83/requirements.txt
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-06-17 03:00:04.748425 clearner-0.9.83/setup.cfg
--rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1831 2023-06-17 02:59:36.000000 clearner-0.9.83/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.182121 clearner-0.9.84/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1993 2022-08-17 03:32:28.000000 clearner-0.9.84/LICENSE
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-07-12 02:50:18.182121 clearner-0.9.84/PKG-INFO
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/clearner.egg-info/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      361 2023-07-12 02:50:18.000000 clearner-0.9.84/clearner.egg-info/PKG-INFO
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3743 2023-07-12 02:50:18.000000 clearner-0.9.84/clearner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        1 2023-07-12 02:50:18.000000 clearner-0.9.84/clearner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       53 2023-07-12 02:50:18.000000 clearner-0.9.84/clearner.egg-info/entry_points.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-07-12 02:50:18.000000 clearner-0.9.84/clearner.egg-info/requires.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        9 2023-07-12 02:50:18.000000 clearner-0.9.84/clearner.egg-info/top_level.txt
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/learner/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       22 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/__init__.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/learner/analysis/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/analysis/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    11442 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/analysis/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7661 2023-07-12 01:47:47.000000 clearner-0.9.84/learner/analysis/plot.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27382 2023-07-12 02:31:11.000000 clearner-0.9.84/learner/analysis/shap.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/learner/api_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/api_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10480 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/api_worker/google_drive.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/learner/callback_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/callback_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9243 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/callback_manager/callback.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/learner/combine/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/combine/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    36131 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/combine/combining_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.170121 clearner-0.9.84/learner/communication/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/communication/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1702 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/communication/communication_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4359 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/communication/email_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.174121 clearner-0.9.84/learner/configuration/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/configuration/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17522 2023-06-17 03:58:58.000000 clearner-0.9.84/learner/configuration/analysis.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9619 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/column.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5138 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/combine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3061 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/communication.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5299 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/configuration.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21627 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/connection.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    31721 2023-06-16 23:56:39.000000 clearner-0.9.84/learner/configuration/data.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39408 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/defaults.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    17803 2023-02-24 19:54:19.000000 clearner-0.9.84/learner/configuration/feature_engineering.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10916 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/model.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14853 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/configuration/outlier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    26515 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/process.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1078 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/configuration/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7012 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/sample.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4701 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/segmenter.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      680 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/configuration/similarities.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     8287 2023-06-02 02:15:58.000000 clearner-0.9.84/learner/configuration/supported_items.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      739 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/configuration/validation.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2113 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/configuration/workspace.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.174121 clearner-0.9.84/learner/data_worker/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/data_worker/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    27945 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15698 2023-02-24 23:02:37.000000 clearner-0.9.84/learner/data_worker/data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7026 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/data_mover.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    52142 2023-04-18 02:21:33.000000 clearner-0.9.84/learner/data_worker/data_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13606 2023-06-02 02:15:58.000000 clearner-0.9.84/learner/data_worker/data_sampler.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23519 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/data_segmenters.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    13742 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/data_set.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    18975 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/deep_tabular_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7996 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/image_data_loader.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10358 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/image_data_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3322 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/data_worker/image_processor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    16872 2023-07-12 02:28:36.000000 clearner-0.9.84/learner/data_worker/output_handler.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.174121 clearner-0.9.84/learner/engines/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/engines/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10891 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/engines/base_deep_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14858 2023-07-12 02:02:04.000000 clearner-0.9.84/learner/engines/base_standard_engine.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1290 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/engines/deep_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1341 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/engines/deep_regressor.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1842 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/engines/engine_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7553 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/engines/image_classifier.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    21014 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/engines/recommender.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    14939 2023-07-12 02:33:26.000000 clearner-0.9.84/learner/engines/standard_engines.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.174121 clearner-0.9.84/learner/feature_engineering/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/feature_engineering/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    19542 2023-02-24 19:54:19.000000 clearner-0.9.84/learner/feature_engineering/feature_engineering.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.178121 clearner-0.9.84/learner/model_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/model_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12192 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    15604 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/deep_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10955 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/deep_loop_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12048 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/deep_regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6419 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/extenders.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    25544 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/image_classifiers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7780 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/layer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1784 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/loss_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6980 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/model_initializer.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2376 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/nn_utils.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2078 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/optimizer_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    39656 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/prediction_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9454 2023-05-19 05:22:49.000000 clearner-0.9.84/learner/model_manager/regressors.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     4802 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/model_manager/scheduler_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      821 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/model_manager/scorers.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    23613 2023-06-02 02:15:58.000000 clearner-0.9.84/learner/model_manager/scoring_manager.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2412 2023-06-02 02:15:58.000000 clearner-0.9.84/learner/model_manager/similarities.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.178121 clearner-0.9.84/learner/outlier_manager/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/outlier_manager/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     7937 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/outlier_manager/outlier_manager.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.178121 clearner-0.9.84/learner/schema/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/schema/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      382 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/schema/credentials_schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      767 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/schema/logging.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       19 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/schema/meta_data.schema.json
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    10921 2023-02-24 19:54:19.000000 clearner-0.9.84/learner/schema/schema.json
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.178121 clearner-0.9.84/learner/setup/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/setup/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     6706 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/setup/logger.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)     2270 2023-07-12 02:49:59.000000 clearner-0.9.84/learner/setup/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1346 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/setup/parser.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3204 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/setup/setup.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.182121 clearner-0.9.84/learner/utilities/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/utilities/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      955 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/utilities/exclude.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     3905 2023-06-02 02:15:58.000000 clearner-0.9.84/learner/utilities/progress_bar.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1218 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/utilities/smtp.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1698 2023-07-12 02:15:44.000000 clearner-0.9.84/learner/utilities/templates.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1333 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/utilities/timer.py
+drwxrwxr-x   0 ramezani  (1000) ramezani  (1000)        0 2023-07-12 02:50:18.182121 clearner-0.9.84/learner/validator/
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)        0 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/validator/__init__.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)    12917 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/validator/column_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5850 2020-12-28 23:50:57.000000 clearner-0.9.84/learner/validator/data_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     9262 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/validator/input_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     5961 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/validator/model_validator.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     2129 2022-08-17 03:32:28.000000 clearner-0.9.84/learner/validator/output_validator.py
+-rwxrwxr-x   0 ramezani  (1000) ramezani  (1000)      296 2022-08-17 03:32:28.000000 clearner-0.9.84/main.py
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)      713 2023-06-02 02:15:58.000000 clearner-0.9.84/requirements.txt
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)       38 2023-07-12 02:50:18.182121 clearner-0.9.84/setup.cfg
+-rw-rw-r--   0 ramezani  (1000) ramezani  (1000)     1831 2023-07-12 02:50:12.000000 clearner-0.9.84/setup.py
```

### Comparing `clearner-0.9.83/LICENSE` & `clearner-0.9.84/LICENSE`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/clearner.egg-info/SOURCES.txt` & `clearner-0.9.84/clearner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/clearner.egg-info/requires.txt` & `clearner-0.9.84/clearner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/analysis/analysis.py` & `clearner-0.9.84/learner/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/analysis/plot.py` & `clearner-0.9.84/learner/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/analysis/shap.py` & `clearner-0.9.84/learner/analysis/shap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sorting, and writing the values as well as creating the narratives and possibly plots. The engines commonly do the
 instantiation and invocation of the classes and methods.
 """
 import pandas as pd
 import numpy as np
 import warnings
 import logging
-from _collections import defaultdict
+from collections import defaultdict
 from numba.core.errors import NumbaDeprecationWarning, NumbaPendingDeprecationWarning
 warnings.filterwarnings('ignore', category=NumbaDeprecationWarning)
 warnings.filterwarnings('ignore', category=NumbaPendingDeprecationWarning)
 import shap
 from shap.plots._beeswarm import pl
 
 from learner.analysis.plot import Plot
@@ -67,15 +67,15 @@
             pos_feat_name = f"positive_feature_{i}"
             neg_val_name = f"negative_value_{i}"
             neg_feat_name = f"negative_feature_{i}"
             value_feature_col_list.extend([pos_val_name, pos_feat_name, neg_val_name, neg_feat_name])
         return value_feature_col_list
 
     @timeit("run shap analysis")
-    def run_shap(self, test_data, tag, index=''):
+    def run_shap(self, test_data, tag, index='', seg_id=''):
         """The main driver method for performing shap analysis calculations. This is the only method that is usually
         called after instantiating the Shap object.
 
         :param test_data: the test dataset. This data set contains the training data as well as the id columns.
         :param tag: the model tag. This is being used to name the files.
         is not being used.
         :param index: if we only loaded test data in chunk, this will be the chunk index
@@ -90,30 +90,30 @@
 
         logging.info("Getting the shap values...")
         logging.info(f"The expected value is {explainer.expected_value}")
         shap_values = explainer.shap_values(test_data[self.models_dict_item["train_features"]])
         # we handle the plots here because in some situations we need only on item in shap_values list and in
         # some situations we need multiple items. Also, we need to plot things before converting shap_values into
         # numpy arrays
-        self.handle_plots(tag, shap_values, test_data)
+        self.handle_plots(tag, shap_values, test_data, seg_id=seg_id)
         shap_values = np.array(shap_values)
 
         # we need the means to use them for storytelling
         self.calculate_the_mean(data=test_data, cols=self.models_dict_item["train_features"])
 
         if len(shap_values.shape) == 3:
             logging.info("It looks like a model with multiple output was run. Learner will process shap values for "
                          "each output")
             for i, class_name in enumerate(self.models_dict_item["model"].classes_):
                 logging.info(f"Processing shap values for class: {class_name}")
-                self.process_shap_data(tag, shap_values[i], test_data, class_name=class_name, index=index)
+                self.process_shap_data(tag, shap_values[i], test_data, class_name=class_name, index=index, seg_id=seg_id)
         else:
-            self.process_shap_data(tag, shap_values, test_data, class_name=None, index=index)
+            self.process_shap_data(tag, shap_values, test_data, class_name=None, index=index, seg_id=seg_id)
 
-    def handle_plots(self, tag, shap_values, test_data):
+    def handle_plots(self, tag, shap_values, test_data, seg_id=''):
         """The main method for using shap library and plotting the data. This method checks if plotting functionality
         was activated or not. If it was activated, it continues with the rest of operations.
 
         :param tag: the model tag. This is being used to name the files.
         :param shap_values: shap values with the same format that comes out of shap library
         :param test_data: the test dataframe
         :return: None
@@ -130,20 +130,26 @@
         except AttributeError:
             class_names = None
 
         # try to make bot bar and dot plots
         for plot_type in ["bar", "dot"]:
             logging.info("Making {plot_type} plot for shap values...".format(plot_type=plot_type))
 
+            if seg_id == '':
+                path = self._conf.model.models_dict[tag]["path"]
+            else:
+                path = self._conf.model.models_dict[tag][seg_id]["path"]
             filename = SHAP_PLOT.format(
-                path=self._conf.model.models_dict[tag]["path"],
+                path=path,
                 output_name=self.conf.workspace.name,
                 tag=str(tag),
                 type=plot_type,
-                sep_timetag=str(self.conf.sep_timetag))
+                sep_timetag=str(self.conf.sep_timetag),
+                seg_id=f"_{seg_id}" if seg_id != '' else seg_id
+            )
             try:
                 # this can fail for dot plot and multi-class classifications problem. In that case, we still want to make
                 # the plots but we need to send the data for each class separately.
                 shap.summary_plot(shap_values,
                                   test_data[self.models_dict_item["train_features"]],
                                   show=False,
                                   max_display=self.conf.analysis.shap_num_features,
@@ -151,32 +157,34 @@
                                   class_names=class_names)
                 Plot.savefig(filename, pl)
                 pl.clf()
             except AssertionError:
                 for i, class_name in enumerate(self.models_dict_item["model"].classes_):
                     logging.info("Plotting shap values for class: {c}".format(c=class_name))
                     filename = SHAP_PLOT_ClASS.format(
-                        path=self._conf.model.models_dict[tag]["path"],
+                        path=path,
                         output_name=self.conf.workspace.name,
                         tag=str(tag),
                         type=plot_type,
                         class_name=class_name,
-                        sep_timetag=str(self.conf.sep_timetag))
+                        sep_timetag=str(self.conf.sep_timetag),
+                        seg_id=f"_{seg_id}" if seg_id != '' else seg_id
+                    )
                     shap.summary_plot(shap_values[i],
                                       test_data[self.models_dict_item["train_features"]],
                                       show=False,
                                       max_display=self.conf.analysis.shap_num_features,
                                       plot_type=plot_type,
                                       class_names=class_names)
 
                     Plot.savefig(filename, pl)
                     pl.clf()
 
     @timeit("process the shap data")
-    def process_shap_data(self, tag, shap_values, test_data, class_name=None, index=''):
+    def process_shap_data(self, tag, shap_values, test_data, class_name=None, index='', seg_id=''):
         """The main method for processing the shap data. This include converting the shap_values numpy arrays in pandas
         dataframe, calling the narrative method to sort the shap values and create the narratives, and saving the final
         data to disk (by calling the write_shap method)
 
         :param tag: the model tag. This is being used to name the files.
         :param shap_values: a numpy array that contain shap values
         :param test_data: the test dataframe
@@ -198,15 +206,15 @@
         else:
             logging.info("Creating narratives for each data point...")
             self.class_name = class_name
 
             shap_df, test_data = parrallelize_dataframes(shap_df, test_data, self.handle_narrative, self.conf.analysis.shap_num_cores)
             # this is the serial code
             # self.create_narrative(shap_df, test_data[self.models_dict_item["train_features"]], class_name=class_name if class_name is not None else "target")
-        self.write_shap(tag, shap_df, test_data[self.conf.column.id_cols], class_name="_{c}".format(c=class_name) if class_name is not None else '', index=index)
+        self.write_shap(tag, shap_df, test_data[self.conf.column.id_cols], class_name="_{c}".format(c=class_name) if class_name is not None else '', index=index, seg_id=seg_id)
 
     @timeit("compute the mean of the columns")
     def calculate_the_mean(self, data, cols):
         """Accept a dataframe and a list of column. If use_training_mean was set to true, get the mean_dict
         (a dictionary in which the key is the column name and the value is the average value of that column), otherwise
         compute the mean of each column and save them to populate mean_dict.
 
@@ -443,15 +451,15 @@
                 narrative.append(feature)
                 narrative.append("(val: {value}, avg: {average:.3f}),".format(value=test_row[feature],
                                                                             average=self.mean_dict[feature]))
 
         return " ".join(narrative)
 
     @timeit("write the shap output")
-    def write_shap(self, tag, shap_df, data, class_name='', index=''):
+    def write_shap(self, tag, shap_df, data, class_name='', index='', seg_id=''):
         """Write the shap dataframe along with any additional columns (typically id columns) to disk. This method also
         makes a call to drop_cols method of the DataProcessor class to drop the unsorted column if not requested.
 
         :param tag: the model tag defined by user in the configuration file.
         :param shap_df: the shap dataframe
         :param data: the additional data to be concatenated with the shap dataframe. This is typically id columns
         :param class_name: the class name in case of multi-class classification problem.
@@ -465,29 +473,34 @@
         if not self.conf.analysis.shap_include_sorted_values:
             DataProcessor.drop_cols(shap_df, self.value_feature_col_list, errors="ignore")
 
         data.reset_index(drop=True, inplace=True)
         shap_df.reset_index(drop=True, inplace=True)
         results = pd.concat([data, shap_df], axis=1, ignore_index=False)
 
-        directory_path = self._conf.model.models_dict[tag]["path"]
+        if seg_id == '':
+            directory_path = self._conf.model.models_dict[tag]["path"]
+        else:
+            directory_path = self._conf.model.models_dict[tag][seg_id]["path"]
         final_filename = SHAP_PATH.format(
             output_name=self._conf.workspace.name,
             tag=str(tag),
             class_name=class_name,
             sep_timetag=str(self._conf.sep_timetag),
-            index=''
+            index='',
+            seg_id=''
         )
 
         filename = SHAP_PATH.format(
             output_name=self._conf.workspace.name,
             tag=str(tag),
             class_name=class_name,
             sep_timetag=str(self._conf.sep_timetag),
-            index=index
+            index=index,
+            seg_id=f"_{seg_id}" if seg_id != '' else seg_id
         )
 
         self.final_filenames[directory_path + final_filename].append(directory_path + filename)
 
         output = OutputHandler(self._conf)
         output.save_file(directory_path, filename, results, add_timetag=False)
         logging.info("Successfully wrote the shap output data")
```

### Comparing `clearner-0.9.83/learner/api_worker/google_drive.py` & `clearner-0.9.84/learner/api_worker/google_drive.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/callback_manager/callback.py` & `clearner-0.9.84/learner/callback_manager/callback.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/combine/combining_manager.py` & `clearner-0.9.84/learner/combine/combining_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/communication/communication_manager.py` & `clearner-0.9.84/learner/communication/communication_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/communication/email_manager.py` & `clearner-0.9.84/learner/communication/email_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/analysis.py` & `clearner-0.9.84/learner/configuration/analysis.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/column.py` & `clearner-0.9.84/learner/configuration/column.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/combine.py` & `clearner-0.9.84/learner/configuration/combine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/communication.py` & `clearner-0.9.84/learner/configuration/communication.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/configuration.py` & `clearner-0.9.84/learner/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/connection.py` & `clearner-0.9.84/learner/configuration/connection.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/data.py` & `clearner-0.9.84/learner/configuration/data.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/defaults.py` & `clearner-0.9.84/learner/configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/feature_engineering.py` & `clearner-0.9.84/learner/configuration/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/model.py` & `clearner-0.9.84/learner/configuration/model.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/outlier.py` & `clearner-0.9.84/learner/configuration/outlier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/process.py` & `clearner-0.9.84/learner/configuration/process.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/recommender.py` & `clearner-0.9.84/learner/configuration/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/sample.py` & `clearner-0.9.84/learner/configuration/sample.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/segmenter.py` & `clearner-0.9.84/learner/configuration/segmenter.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/similarities.py` & `clearner-0.9.84/learner/configuration/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/supported_items.py` & `clearner-0.9.84/learner/configuration/supported_items.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/validation.py` & `clearner-0.9.84/learner/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/configuration/workspace.py` & `clearner-0.9.84/learner/configuration/workspace.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_loader.py` & `clearner-0.9.84/learner/data_worker/data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_manager.py` & `clearner-0.9.84/learner/data_worker/data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_mover.py` & `clearner-0.9.84/learner/data_worker/data_mover.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_processor.py` & `clearner-0.9.84/learner/data_worker/data_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_sampler.py` & `clearner-0.9.84/learner/data_worker/data_sampler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_segmenters.py` & `clearner-0.9.84/learner/data_worker/data_segmenters.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/data_set.py` & `clearner-0.9.84/learner/data_worker/data_set.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/deep_tabular_data_manager.py` & `clearner-0.9.84/learner/data_worker/deep_tabular_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/image_data_loader.py` & `clearner-0.9.84/learner/data_worker/image_data_loader.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/image_data_manager.py` & `clearner-0.9.84/learner/data_worker/image_data_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/image_processor.py` & `clearner-0.9.84/learner/data_worker/image_processor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/data_worker/output_handler.py` & `clearner-0.9.84/learner/data_worker/output_handler.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/base_deep_engine.py` & `clearner-0.9.84/learner/engines/base_deep_engine.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/base_standard_engine.py` & `clearner-0.9.84/learner/engines/base_standard_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,26 +249,26 @@
                 logging.info("Combining the predictions of different models using 'triad' method and test data")
                 if not self.combiner:
                     logging.critical("It looks like combiner is not loaded. Exiting...")
                     sys.exit(1)
 
                 self.combiner.transform(data_type="test")
 
-    def handle_shap(self, mdl, data, tag, index=''):
+    def handle_shap(self, mdl, data, tag, index='', seg_id=''):
         """Instantiate appropriate objects and call the necessary methods to perform various analysis.
 
         :param mdl: an trained model
         :param data: a pandas dataframe. This could be validation or test datasets
         :param tag: the model tag in the models_dict
         :return: None
         """
         if self._conf.analysis.shap_activate:
             if self.shap is None:
                 self.shap = Shap(mdl, self._conf, self.processor)
-            self.shap.run_shap(data, tag, index=index)
+            self.shap.run_shap(data, tag, index=index, seg_id=seg_id)
 
     def handle_predictions_vs_actuals(self, models_dict):
         """Accept a models_dict, iterate through it, and call handle_predictions_vs_actuals_plot method in the
         Analysis class tp plot predictions vs actuals graph. The handle_predictions_vs_actuals_plot method will
         figure out where the prediction and actual data are located.
 
         :param models_dict: a models_dict. This dictionary is a complete dictionary not only one item.
```

### Comparing `clearner-0.9.83/learner/engines/deep_classifier.py` & `clearner-0.9.84/learner/engines/deep_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/deep_regressor.py` & `clearner-0.9.84/learner/engines/deep_regressor.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/engine_manager.py` & `clearner-0.9.84/learner/engines/engine_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/image_classifier.py` & `clearner-0.9.84/learner/engines/image_classifier.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/recommender.py` & `clearner-0.9.84/learner/engines/recommender.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/engines/standard_engines.py` & `clearner-0.9.84/learner/engines/standard_engines.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,15 @@
                                         mdl=mdl,
                                         seg_id=seg_id,
                                         data_type="validation",
                                         add_version=self._conf.model.version_activate,
                                         version_name=self._conf.model.version_version_name,
                                         version_column_name=self._conf.model.version_column_name
                                         )
+            self.handle_shap(mdl, validation_manager.data, tag, seg_id=seg_id)
 
     def predict_test(self, seg_id=None, seg_border=None):
         """Use the trained models to make predictions. Making predictions are performed by iterating through the
         test dataset. The test dataset can be very large and we process it in chunks.
 
         :param seg_id: the seg id
         :param seg_border: the upper boundary of the seg
@@ -293,13 +294,17 @@
                                             mdl,
                                             seg_id=seg_id,
                                             data_type="test",
                                             add_version=self._conf.model.version_activate,
                                             version_name=self._conf.model.version_version_name,
                                             version_column_name=self._conf.model.version_column_name
                                             )
+                self.handle_shap(mdl, test_data, tag, index, seg_id)
 
             # keep track of number of rows in test dataset for validation purposes
             self.conf.model.nrows_score += chunk.shape[0]
 
         output = OutputHandler(self._conf, data_type="test")
         output.concat_chunk_csv(num_chunks, self.models_dict, seg_id)
+        if self.shap is not None:
+            output.concat_dict_of_csv_files(self.shap.final_filenames)
+
```

### Comparing `clearner-0.9.83/learner/feature_engineering/feature_engineering.py` & `clearner-0.9.84/learner/feature_engineering/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/classifiers.py` & `clearner-0.9.84/learner/model_manager/classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/deep_classifiers.py` & `clearner-0.9.84/learner/model_manager/deep_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/deep_loop_manager.py` & `clearner-0.9.84/learner/model_manager/deep_loop_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/deep_regressors.py` & `clearner-0.9.84/learner/model_manager/deep_regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/extenders.py` & `clearner-0.9.84/learner/model_manager/extenders.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/image_classifiers.py` & `clearner-0.9.84/learner/model_manager/image_classifiers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/layer_manager.py` & `clearner-0.9.84/learner/model_manager/layer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/loss_manager.py` & `clearner-0.9.84/learner/model_manager/loss_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/model_initializer.py` & `clearner-0.9.84/learner/model_manager/model_initializer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/nn_utils.py` & `clearner-0.9.84/learner/model_manager/nn_utils.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/optimizer_manager.py` & `clearner-0.9.84/learner/model_manager/optimizer_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/prediction_manager.py` & `clearner-0.9.84/learner/model_manager/prediction_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/regressors.py` & `clearner-0.9.84/learner/model_manager/regressors.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/scheduler_manager.py` & `clearner-0.9.84/learner/model_manager/scheduler_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/scorers.py` & `clearner-0.9.84/learner/model_manager/scorers.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/scoring_manager.py` & `clearner-0.9.84/learner/model_manager/scoring_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/model_manager/similarities.py` & `clearner-0.9.84/learner/model_manager/similarities.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/outlier_manager/outlier_manager.py` & `clearner-0.9.84/learner/outlier_manager/outlier_manager.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/schema/logging.json` & `clearner-0.9.84/learner/schema/logging.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/schema/schema.json` & `clearner-0.9.84/learner/schema/schema.json`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/setup/logger.py` & `clearner-0.9.84/learner/setup/logger.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/setup/main.py` & `clearner-0.9.84/learner/setup/main.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/setup/parser.py` & `clearner-0.9.84/learner/setup/parser.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/setup/setup.py` & `clearner-0.9.84/learner/setup/setup.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/utilities/exclude.py` & `clearner-0.9.84/learner/utilities/exclude.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/utilities/progress_bar.py` & `clearner-0.9.84/learner/utilities/progress_bar.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/utilities/smtp.py` & `clearner-0.9.84/learner/utilities/smtp.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/utilities/templates.py` & `clearner-0.9.84/learner/utilities/templates.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 LOAD_MODEL_PATH_SEG = "{path}{prefix}_{seg_id}{sep_timetag}{ext}"
 
 FEATURE_IMPORTANCE_PATH = "{output_name}_{tag}_feature_importance{sep_timetag}"
 FEATURE_IMPORTANCE_PATH_SEG = "{output_name}_{tag}_{seg_id}_feature_importance{sep_timetag}"
 
 PREDICTIONS_VS_ACTUALS_PLOT = "{path}{output_name}_{tag}_predictions_vs_actuals{sep_timetag}.png"
 
-SHAP_PATH = "{output_name}_{tag}_shap_values{class_name}{sep_timetag}{index}.csv"
-SHAP_PLOT = "{path}{output_name}_{tag}_shap_{type}{sep_timetag}.png"
-SHAP_PLOT_ClASS = "{path}{output_name}_{tag}_shap_{type}_{class_name}{sep_timetag}.png"
+SHAP_PATH = "{output_name}_{tag}_shap_values{class_name}{sep_timetag}{index}{seg_id}.csv"
+SHAP_PLOT = "{path}{output_name}_{tag}_shap_{type}{sep_timetag}{seg_id}.png"
+SHAP_PLOT_ClASS = "{path}{output_name}_{tag}_shap_{type}_{class_name}{sep_timetag}{seg_id}.png"
 
 TRAIN_VALIDATION_SPLIT = "{output_name}_{dtype}_split{sep_timetag}.{format}"
 
 LEARNING_RATE = "{path}{output_name}_{tag}_learning_rate{sep_timetag}.png"
```

### Comparing `clearner-0.9.83/learner/utilities/timer.py` & `clearner-0.9.84/learner/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/validator/column_validator.py` & `clearner-0.9.84/learner/validator/column_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/validator/data_validator.py` & `clearner-0.9.84/learner/validator/data_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/validator/input_validator.py` & `clearner-0.9.84/learner/validator/input_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/validator/model_validator.py` & `clearner-0.9.84/learner/validator/model_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/learner/validator/output_validator.py` & `clearner-0.9.84/learner/validator/output_validator.py`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/requirements.txt` & `clearner-0.9.84/requirements.txt`

 * *Files identical despite different names*

### Comparing `clearner-0.9.83/setup.py` & `clearner-0.9.84/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def compile_learner():
     """Go through each package and modules, and compile them.
 
     :return: None
     """
     setup(
         name='clearner',
-        version='0.9.83',
+        version='0.9.84',
         description="Learner is a software platform for building production-ready machine learning models without writing any codes.",
         author="Prizmi LLC",
         author_email="contact@prizmi.ai",
         python_requires='>=3.8,<3.10',
         url="https://prizmi.ai/learner/home",
         license="Other",
         build_dir="build",
```

