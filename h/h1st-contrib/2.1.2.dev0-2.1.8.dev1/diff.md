# Comparing `tmp/h1st_contrib-2.1.2.dev0.tar.gz` & `tmp/h1st_contrib-2.1.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h1st_contrib-2.1.2.dev0.tar", max compression
+gzip compressed data, was "h1st_contrib-2.1.8.dev1.tar", max compression
```

## Comparing `h1st_contrib-2.1.2.dev0.tar` & `h1st_contrib-2.1.8.dev1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      550 2023-01-10 18:34:36.000000 h1st_contrib-2.1.2.dev0/LICENSE
--rw-r--r--   0        0        0     4111 2023-01-10 18:34:37.000000 h1st_contrib-2.1.2.dev0/README.md
--rw-r--r--   0        0        0      253 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/data_mgmt/__init__.py
--rw-r--r--   0        0        0     6153 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/data_mgmt/equipment_parquet_data.py
--rw-r--r--   0        0        0      659 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/__init__.py
--rwxr-xr-x   0        0        0     8114 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/base.py
--rwxr-xr-x   0        0        0     5298 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/__init__.py
--rw-r--r--   0        0        0     1426 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/ensemble/basic.py
--rw-r--r--   0        0        0    34370 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/student/timeseries_dl.py
--rw-r--r--   0        0        0     1450 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/teacher/base.py
--rw-r--r--   0        0        0     1464 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/__init__.py
--rw-r--r--   0        0        0      335 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/__init__.py
--rwxr-xr-x   0        0        0     9979 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/build.py
--rwxr-xr-x   0        0        0     5477 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/exec.py
--rwxr-xr-x   0        0        0     3373 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/tune.py
--rw-r--r--   0        0        0        0 2023-01-10 18:34:49.000000 h1st_contrib-2.1.2.dev0/h1st/core/__init__.py
--rw-r--r--   0        0        0     1808 2023-01-10 18:34:49.000000 h1st_contrib-2.1.2.dev0/h1st/core/context.py
--rw-r--r--   0        0        0     6396 2023-01-10 18:34:50.000000 h1st_contrib-2.1.2.dev0/h1st/core/viz.py
--rw-r--r--   0        0        0        0 2023-01-10 18:34:50.000000 h1st_contrib-2.1.2.dev0/h1st/exceptions/__init__.py
--rw-r--r--   0        0        0      131 2023-01-10 18:34:50.000000 h1st_contrib-2.1.2.dev0/h1st/exceptions/exception.py
--rw-r--r--   0        0        0      111 2023-01-10 18:34:50.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/README.md
--rw-r--r--   0        0        0        0 2023-01-10 18:34:50.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/__init__.py
--rw-r--r--   0        0        0    11871 2023-01-10 18:34:51.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/h1flow.py
--rw-r--r--   0        0        0    12139 2023-01-10 18:34:51.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/h1step.py
--rw-r--r--   0        0        0     3039 2023-01-10 18:34:52.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/h1step_containable.py
--rw-r--r--   0        0        0      301 2023-01-10 18:34:53.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/temp_step.py
--rw-r--r--   0        0        0        0 2023-01-10 18:34:53.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/ui/__init__.py
--rw-r--r--   0        0        0      394 2023-01-10 18:34:53.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/ui/has_ui.py
--rw-r--r--   0        0        0      945 2023-01-10 18:34:54.000000 h1st_contrib-2.1.2.dev0/h1st/h1flow/ui/has_web_ui.py
--rw-r--r--   0        0        0      175 2023-01-10 18:34:54.000000 h1st_contrib-2.1.2.dev0/h1st/metadata.json
--rw-r--r--   0        0        0      391 2023-01-10 18:34:54.000000 h1st_contrib-2.1.2.dev0/h1st/model/README.md
--rw-r--r--   0        0        0        0 2023-01-10 18:34:54.000000 h1st_contrib-2.1.2.dev0/h1st/model/__init__.py
--rw-r--r--   0        0        0      769 2023-05-12 11:19:04.000000 h1st_contrib-2.1.2.dev0/h1st/model/ml/xgboost/classifier.py
--rw-r--r--   0        0        0    15299 2023-05-12 11:19:04.000000 h1st_contrib-2.1.2.dev0/h1st/model/ml/xgboost/regression.py
--rw-r--r--   0        0        0     5126 2023-03-05 19:48:21.000000 h1st_contrib-2.1.2.dev0/h1st/model/ml/xgboost/utils.py
--rw-r--r--   0        0        0     3945 2023-03-05 19:48:21.000000 h1st_contrib-2.1.2.dev0/h1st/model/model.py
--rw-r--r--   0        0        0     5657 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/model/oracle/oracle.py
--rw-r--r--   0        0        0        0 2023-01-10 18:35:01.000000 h1st_contrib-2.1.2.dev0/h1st/model/repository/__init__.py
--rw-r--r--   0        0        0     4052 2023-01-10 18:35:03.000000 h1st_contrib-2.1.2.dev0/h1st/model/repository/explorer.py
--rw-r--r--   0        0        0    22687 2023-03-05 19:48:21.000000 h1st_contrib-2.1.2.dev0/h1st/model/repository/model_repository.py
--rw-r--r--   0        0        0      797 2023-01-10 18:35:03.000000 h1st_contrib-2.1.2.dev0/h1st/model/repository/storage/base.py
--rw-r--r--   0        0        0     2924 2023-01-10 18:35:03.000000 h1st_contrib-2.1.2.dev0/h1st/model/repository/storage/local.py
--rw-r--r--   0        0        0     2563 2023-01-10 18:35:04.000000 h1st_contrib-2.1.2.dev0/h1st/model/repository/storage/s3.py
--rw-r--r--   0        0        0        0 2023-01-10 18:35:04.000000 h1st_contrib-2.1.2.dev0/h1st/trust/__init__.py
--rw-r--r--   0        0        0      931 2023-01-10 18:35:04.000000 h1st_contrib-2.1.2.dev0/h1st/trust/auditable.py
--rw-r--r--   0        0        0      116 2023-01-10 18:35:04.000000 h1st_contrib-2.1.2.dev0/h1st/trust/debiasable.py
--rw-r--r--   0        0        0      567 2023-01-10 18:35:04.000000 h1st_contrib-2.1.2.dev0/h1st/trust/decision.py
--rw-r--r--   0        0        0     1433 2023-01-10 18:35:05.000000 h1st_contrib-2.1.2.dev0/h1st/trust/describable.py
--rw-r--r--   0        0        0     1619 2023-01-10 18:35:05.000000 h1st_contrib-2.1.2.dev0/h1st/trust/describer.py
--rw-r--r--   0        0        0     1140 2023-01-10 18:35:05.000000 h1st_contrib-2.1.2.dev0/h1st/trust/enums.py
--rw-r--r--   0        0        0     1420 2023-01-10 18:35:06.000000 h1st_contrib-2.1.2.dev0/h1st/trust/explainable.py
--rw-r--r--   0        0        0     1045 2023-01-10 18:35:06.000000 h1st_contrib-2.1.2.dev0/h1st/trust/explainer.py
--rw-r--r--   0        0        0      957 2023-01-10 18:35:06.000000 h1st_contrib-2.1.2.dev0/h1st/trust/lime_model_explainer.py
--rw-r--r--   0        0        0       54 2023-01-10 18:35:07.000000 h1st_contrib-2.1.2.dev0/h1st/trust/output_formatters.py
--rw-r--r--   0        0        0      641 2023-01-10 18:35:07.000000 h1st_contrib-2.1.2.dev0/h1st/trust/shap_model_describer.py
--rw-r--r--   0        0        0      315 2023-01-10 18:35:07.000000 h1st_contrib-2.1.2.dev0/h1st/trust/trustable.py
--rw-r--r--   0        0        0      236 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/__init__.py
--rw-r--r--   0        0        0    17201 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/_abstract.py
--rw-r--r--   0        0        0    12825 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/pandas.py
--rw-r--r--   0        0        0    97784 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/parquet.py
--rw-r--r--   0        0        0     3773 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_types/arrow.py
--rw-r--r--   0        0        0     1402 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_types/numpy_pandas.py
--rw-r--r--   0        0        0      467 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_types/python.py
--rwxr-xr-x   0        0        0     3962 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/data_types/spark_sql.py
--rw-r--r--   0        0        0       37 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/debug.py
--rw-r--r--   0        0        0     1123 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/default_dict.py
--rw-r--r--   0        0        0     9272 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/fs.py
--rw-r--r--   0        0        0      825 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/iter.py
--rw-r--r--   0        0        0     1238 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/log.py
--rw-r--r--   0        0        0    17177 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/namespace.py
--rwxr-xr-x   0        0        0      314 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/path.py
--rw-r--r--   0        0        0     4958 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/s3.py
--rw-r--r--   0        0        0      855 2023-05-12 11:18:59.000000 h1st_contrib-2.1.2.dev0/h1st/utils/tools.py
--rw-r--r--   0        0        0     1446 2023-06-16 05:08:08.439186 h1st_contrib-2.1.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 h1st_contrib-2.1.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-01-10 18:34:36.000000 h1st_contrib-2.1.8.dev1/LICENSE
+-rw-r--r--   0        0        0     4111 2023-01-10 18:34:37.000000 h1st_contrib-2.1.8.dev1/README.md
+-rw-r--r--   0        0        0      253 2023-07-06 06:50:26.645350 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/data_mgmt/__init__.py
+-rw-r--r--   0        0        0     6153 2023-07-06 06:50:26.646238 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/data_mgmt/equipment_parquet_data.py
+-rw-r--r--   0        0        0      659 2023-07-06 06:50:26.647017 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/__init__.py
+-rwxr-xr-x   0        0        0     8114 2023-07-06 06:50:26.647864 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/base.py
+-rwxr-xr-x   0        0        0     5298 2023-07-06 06:50:26.648548 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-06 06:50:26.649011 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/ensemble/basic.py
+-rw-r--r--   0        0        0    34370 2023-07-06 06:50:26.649560 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/student/timeseries_dl.py
+-rw-r--r--   0        0        0     1450 2023-07-06 06:50:26.649913 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/teacher/base.py
+-rw-r--r--   0        0        0     1464 2023-07-06 06:50:26.650278 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/__init__.py
+-rw-r--r--   0        0        0      335 2023-07-06 06:50:26.650623 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/__init__.py
+-rwxr-xr-x   0        0        0     9979 2023-07-06 06:50:26.651201 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/build.py
+-rwxr-xr-x   0        0        0     5477 2023-07-06 06:50:26.651890 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/exec.py
+-rwxr-xr-x   0        0        0     3373 2023-07-06 06:50:26.652370 h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/tune.py
+-rw-r--r--   0        0        0        0 2023-01-10 18:34:49.000000 h1st_contrib-2.1.8.dev1/h1st/core/__init__.py
+-rw-r--r--   0        0        0     1808 2023-01-10 18:34:49.000000 h1st_contrib-2.1.8.dev1/h1st/core/context.py
+-rw-r--r--   0        0        0     6396 2023-01-10 18:34:50.000000 h1st_contrib-2.1.8.dev1/h1st/core/viz.py
+-rw-r--r--   0        0        0        0 2023-01-10 18:34:50.000000 h1st_contrib-2.1.8.dev1/h1st/exceptions/__init__.py
+-rw-r--r--   0        0        0      131 2023-01-10 18:34:50.000000 h1st_contrib-2.1.8.dev1/h1st/exceptions/exception.py
+-rw-r--r--   0        0        0      111 2023-01-10 18:34:50.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/README.md
+-rw-r--r--   0        0        0        0 2023-01-10 18:34:50.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/__init__.py
+-rw-r--r--   0        0        0    11871 2023-01-10 18:34:51.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/h1flow.py
+-rw-r--r--   0        0        0    12139 2023-01-10 18:34:51.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/h1step.py
+-rw-r--r--   0        0        0     3039 2023-01-10 18:34:52.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/h1step_containable.py
+-rw-r--r--   0        0        0      301 2023-01-10 18:34:53.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/temp_step.py
+-rw-r--r--   0        0        0        0 2023-01-10 18:34:53.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/ui/__init__.py
+-rw-r--r--   0        0        0      394 2023-01-10 18:34:53.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/ui/has_ui.py
+-rw-r--r--   0        0        0      945 2023-01-10 18:34:54.000000 h1st_contrib-2.1.8.dev1/h1st/h1flow/ui/has_web_ui.py
+-rw-r--r--   0        0        0      175 2023-01-10 18:34:54.000000 h1st_contrib-2.1.8.dev1/h1st/metadata.json
+-rw-r--r--   0        0        0      391 2023-01-10 18:34:54.000000 h1st_contrib-2.1.8.dev1/h1st/model/README.md
+-rw-r--r--   0        0        0        0 2023-01-10 18:34:54.000000 h1st_contrib-2.1.8.dev1/h1st/model/__init__.py
+-rw-r--r--   0        0        0      769 2023-05-12 11:19:04.000000 h1st_contrib-2.1.8.dev1/h1st/model/ml/xgboost/classifier.py
+-rw-r--r--   0        0        0    15299 2023-05-12 11:19:04.000000 h1st_contrib-2.1.8.dev1/h1st/model/ml/xgboost/regression.py
+-rw-r--r--   0        0        0     5126 2023-03-05 19:48:21.000000 h1st_contrib-2.1.8.dev1/h1st/model/ml/xgboost/utils.py
+-rw-r--r--   0        0        0     3960 2023-07-06 06:50:46.813543 h1st_contrib-2.1.8.dev1/h1st/model/model.py
+-rw-r--r--   0        0        0     5657 2023-07-06 06:50:26.653506 h1st_contrib-2.1.8.dev1/h1st/model/oracle/oracle.py
+-rw-r--r--   0        0        0        0 2023-01-10 18:35:01.000000 h1st_contrib-2.1.8.dev1/h1st/model/repository/__init__.py
+-rw-r--r--   0        0        0     4052 2023-01-10 18:35:03.000000 h1st_contrib-2.1.8.dev1/h1st/model/repository/explorer.py
+-rw-r--r--   0        0        0    22920 2023-07-06 06:50:46.813861 h1st_contrib-2.1.8.dev1/h1st/model/repository/model_repository.py
+-rw-r--r--   0        0        0      797 2023-01-10 18:35:03.000000 h1st_contrib-2.1.8.dev1/h1st/model/repository/storage/base.py
+-rw-r--r--   0        0        0     2924 2023-01-10 18:35:03.000000 h1st_contrib-2.1.8.dev1/h1st/model/repository/storage/local.py
+-rw-r--r--   0        0        0     2805 2023-07-06 06:50:46.814045 h1st_contrib-2.1.8.dev1/h1st/model/repository/storage/s3.py
+-rw-r--r--   0        0        0        0 2023-01-10 18:35:04.000000 h1st_contrib-2.1.8.dev1/h1st/trust/__init__.py
+-rw-r--r--   0        0        0      931 2023-01-10 18:35:04.000000 h1st_contrib-2.1.8.dev1/h1st/trust/auditable.py
+-rw-r--r--   0        0        0      116 2023-01-10 18:35:04.000000 h1st_contrib-2.1.8.dev1/h1st/trust/debiasable.py
+-rw-r--r--   0        0        0      567 2023-01-10 18:35:04.000000 h1st_contrib-2.1.8.dev1/h1st/trust/decision.py
+-rw-r--r--   0        0        0     1433 2023-01-10 18:35:05.000000 h1st_contrib-2.1.8.dev1/h1st/trust/describable.py
+-rw-r--r--   0        0        0     1619 2023-01-10 18:35:05.000000 h1st_contrib-2.1.8.dev1/h1st/trust/describer.py
+-rw-r--r--   0        0        0     1140 2023-01-10 18:35:05.000000 h1st_contrib-2.1.8.dev1/h1st/trust/enums.py
+-rw-r--r--   0        0        0     1420 2023-01-10 18:35:06.000000 h1st_contrib-2.1.8.dev1/h1st/trust/explainable.py
+-rw-r--r--   0        0        0     1045 2023-01-10 18:35:06.000000 h1st_contrib-2.1.8.dev1/h1st/trust/explainer.py
+-rw-r--r--   0        0        0      957 2023-01-10 18:35:06.000000 h1st_contrib-2.1.8.dev1/h1st/trust/lime_model_explainer.py
+-rw-r--r--   0        0        0       54 2023-01-10 18:35:07.000000 h1st_contrib-2.1.8.dev1/h1st/trust/output_formatters.py
+-rw-r--r--   0        0        0      641 2023-01-10 18:35:07.000000 h1st_contrib-2.1.8.dev1/h1st/trust/shap_model_describer.py
+-rw-r--r--   0        0        0      315 2023-01-10 18:35:07.000000 h1st_contrib-2.1.8.dev1/h1st/trust/trustable.py
+-rw-r--r--   0        0        0      236 2023-07-06 06:50:26.654652 h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/__init__.py
+-rw-r--r--   0        0        0    17201 2023-07-06 06:50:26.655213 h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/_abstract.py
+-rw-r--r--   0        0        0    12825 2023-07-06 06:50:26.655806 h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/pandas.py
+-rw-r--r--   0        0        0    97784 2023-07-06 06:50:26.656597 h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/parquet.py
+-rw-r--r--   0        0        0     3773 2023-07-06 06:50:26.657142 h1st_contrib-2.1.8.dev1/h1st/utils/data_types/arrow.py
+-rw-r--r--   0        0        0     1404 2023-07-14 04:24:41.586498 h1st_contrib-2.1.8.dev1/h1st/utils/data_types/numpy_pandas.py
+-rw-r--r--   0        0        0      467 2023-07-06 06:50:26.658036 h1st_contrib-2.1.8.dev1/h1st/utils/data_types/python.py
+-rwxr-xr-x   0        0        0     3962 2023-07-06 06:50:26.658138 h1st_contrib-2.1.8.dev1/h1st/utils/data_types/spark_sql.py
+-rw-r--r--   0        0        0       37 2023-07-06 06:50:26.658240 h1st_contrib-2.1.8.dev1/h1st/utils/debug.py
+-rw-r--r--   0        0        0     1123 2023-07-06 06:50:26.658339 h1st_contrib-2.1.8.dev1/h1st/utils/default_dict.py
+-rw-r--r--   0        0        0     9272 2023-07-06 06:50:26.658851 h1st_contrib-2.1.8.dev1/h1st/utils/fs.py
+-rw-r--r--   0        0        0      825 2023-07-06 06:50:26.659476 h1st_contrib-2.1.8.dev1/h1st/utils/iter.py
+-rw-r--r--   0        0        0     1238 2023-07-06 06:50:26.659587 h1st_contrib-2.1.8.dev1/h1st/utils/log.py
+-rw-r--r--   0        0        0    17177 2023-07-06 06:50:26.660032 h1st_contrib-2.1.8.dev1/h1st/utils/namespace.py
+-rwxr-xr-x   0        0        0      314 2023-07-06 06:50:26.660618 h1st_contrib-2.1.8.dev1/h1st/utils/path.py
+-rw-r--r--   0        0        0     4958 2023-07-06 06:50:26.661037 h1st_contrib-2.1.8.dev1/h1st/utils/s3.py
+-rw-r--r--   0        0        0      855 2023-07-06 06:50:26.661351 h1st_contrib-2.1.8.dev1/h1st/utils/tools.py
+-rw-r--r--   0        0        0     1449 2023-07-14 04:26:53.795459 h1st_contrib-2.1.8.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 h1st_contrib-2.1.8.dev1/PKG-INFO
```

### Comparing `h1st_contrib-2.1.2.dev0/LICENSE` & `h1st_contrib-2.1.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/README.md` & `h1st_contrib-2.1.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/data_mgmt/equipment_parquet_data.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/data_mgmt/equipment_parquet_data.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/__init__.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/base.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/base.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/__init__.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/ensemble/basic.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/ensemble/basic.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/student/timeseries_dl.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/student/timeseries_dl.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/models/oracle/teacher/base.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/models/oracle/teacher/base.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/__init__.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/build.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/build.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/exec.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/exec.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/contrib/pmfp/tools/oracle/tune.py` & `h1st_contrib-2.1.8.dev1/h1st/contrib/pmfp/tools/oracle/tune.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/core/context.py` & `h1st_contrib-2.1.8.dev1/h1st/core/context.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/core/viz.py` & `h1st_contrib-2.1.8.dev1/h1st/core/viz.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/h1flow/h1flow.py` & `h1st_contrib-2.1.8.dev1/h1st/h1flow/h1flow.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/h1flow/h1step.py` & `h1st_contrib-2.1.8.dev1/h1st/h1flow/h1step.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/h1flow/h1step_containable.py` & `h1st_contrib-2.1.8.dev1/h1st/h1flow/h1step_containable.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/h1flow/ui/has_web_ui.py` & `h1st_contrib-2.1.8.dev1/h1st/h1flow/ui/has_web_ui.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/ml/xgboost/classifier.py` & `h1st_contrib-2.1.8.dev1/h1st/model/ml/xgboost/classifier.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/ml/xgboost/regression.py` & `h1st_contrib-2.1.8.dev1/h1st/model/ml/xgboost/regression.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/ml/xgboost/utils.py` & `h1st_contrib-2.1.8.dev1/h1st/model/ml/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/model.py` & `h1st_contrib-2.1.8.dev1/h1st/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,33 +44,33 @@
     """
     def __init__(self):
         super().__init__()
         self.stats = {}
         self.metrics = {}
         self.base_model = None
 
-    def persist(self, version=None) -> str:
+    def persist(self, path: str, version: str = None) -> str:
         """
         Persist this model's properties to the ModelRepository. Currently, only `stats`, `metrics`, `model` properties are supported.
 
         `model` property could be single model, list or dict of models
         Currently, only sklearn and tensorflow-keras are supported.
 
         :param version: model version, leave blank for autogeneration
         :returns: model version
         """
-        repo = ModelRepository.get_model_repo(self)
+        repo = ModelRepository(storage=path)
         return repo.persist(model=self, version=version)
 
-    def load(self, version: str = None) -> Any:
+    def load(self, path: str, version: str = None) -> Any:
         """
         Load parameters from the specified `version` from the ModelRepository.
         Leave version blank to load latest version.
         """
-        repo = ModelRepository.get_model_repo(self)
+        repo = ModelRepository(storage=path)
         repo.load(model=self, version=version)
 
         return self
 
     def train(self, data: Dict[str, Any] = None) -> None:
         """
         Implement logic to create the corresponding MLModel, including both training and evaluation.
```

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/oracle/oracle.py` & `h1st_contrib-2.1.8.dev1/h1st/model/oracle/oracle.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/repository/explorer.py` & `h1st_contrib-2.1.8.dev1/h1st/model/repository/explorer.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/repository/model_repository.py` & `h1st_contrib-2.1.8.dev1/h1st/model/repository/model_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,16 @@
 
                 self._storage.set_obj(
                     self._get_key(model, "latest"),
                     version,
                 )
 
                 model.version = version
+        except Exception as e:
+            logger.exception(f'Error persisting model {model} version {version}: {e}')
         finally:
             dir_util.remove_tree(tmpdir)
 
         return version
 
     def load(self, model, version=None):
         """
@@ -459,14 +461,16 @@
 
             with open(tar_file, "wb") as f:
                 f.write(self._storage.get_bytes(self._get_key(model, version)))
 
             _tar_extract(tar_file, serialized_dir)
             self._serder.deserialize(model, serialized_dir)
             model.version = version
+        except Exception as e:
+            logger.exception(f'Error loading model {model} version {version}: {e}')
         finally:
             # We get error from Tensorflow telling that it could not find the folder
             # Unsuccessful TensorSliceReader constructor: Failed to get matching files on
             # /var/folders/wb/40304xlx477cfjzbk386l2gr0000gn/T/tmpwcrvm2e2/model/weights:
             # Not found: /var/folders/wb/40304xlx477cfjzbk386l2gr0000gn/T/tmpwcrvm2e2/model; No such file or directory [Op:RestoreV2]
             #
             # dir_util.remove_tree(tmpdir)
```

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/repository/storage/base.py` & `h1st_contrib-2.1.8.dev1/h1st/model/repository/storage/base.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/repository/storage/local.py` & `h1st_contrib-2.1.8.dev1/h1st/model/repository/storage/local.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/model/repository/storage/s3.py` & `h1st_contrib-2.1.8.dev1/h1st/model/repository/storage/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, NoReturn
 import cloudpickle
 import s3fs
 from h1st.model.repository.storage.base import Storage
+from loguru import logger
 
 
 class S3Storage(Storage):
     """
     Provide data storage on top of AWS S3
     """
 
-    def __init__(self, bucket_name: str = "", prefix: str = ""):
+    def __init__(self, bucket_name: str = None, prefix: str = None):
         """
         :param bucket_name: s3 bucket name to store data into
         :param prefix: s3 object prefix, leave blank to store at bucket root
         """
         self.bucket_name = bucket_name
         self.prefix = prefix
         self.fs = s3fs.S3FileSystem()
@@ -21,53 +22,59 @@
     def get_obj(self, name: str) -> Any:
         """
         Retrieve object value
 
         :param name: object name
         """
         key = self._to_key(name)
+        logger.info(f"---Loading obj {key} from S3")
+
         try:
             with self.fs.open(key, 'rb') as f:
                 return cloudpickle.load(f)
         except FileNotFoundError as ex:
             raise KeyError(name) from ex
 
     def get_bytes(self, name) -> bytes:
         """
         Retrieve object value in bytes
 
         :param name: object name
         """
         key = self._to_key(name)
+        logger.info(f"---Loading bytes {key} from S3")
+
         try:
             with self.fs.open(key, 'rb') as f:
                 return f.read()
         except FileNotFoundError as ex:
             raise KeyError(name) from ex
 
     def set_obj(self, name: str, value: Any) -> NoReturn:
         """
         Set key value to a python object
 
         :param name: object name
         :param value: value in python object
         """
         key = self._to_key(name)
+        logger.info(f"---Saving obj {key} to S3")
 
         with self.fs.open(key, 'wb') as f:
             return cloudpickle.dump(value, f)
 
     def set_bytes(self, name: str, value: bytes) -> NoReturn:
         """
         Set a key value to a list of bytes
 
         :param name: object name
         :param value: value in bytes
         """
         key = self._to_key(name)
+        logger.info(f"---Saving bytes {key} to S3")
 
         with self.fs.open(key, 'wb') as f:
             f.write(value)
 
     def exists(self, name: str) -> bool:
         """
         Return true if object exists in the storage
```

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/auditable.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/auditable.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/decision.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/decision.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/describable.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/describable.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/describer.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/describer.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/enums.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/enums.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/explainable.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/explainable.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/explainer.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/explainer.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/lime_model_explainer.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/lime_model_explainer.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/trust/shap_model_describer.py` & `h1st_contrib-2.1.8.dev1/h1st/trust/shap_model_describer.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/_abstract.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/_abstract.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/pandas.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/pandas.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/data_proc/parquet.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/data_proc/parquet.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/data_types/arrow.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/data_types/arrow.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/data_types/numpy_pandas.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/data_types/numpy_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 NUMPY_FLOAT_TYPES: Tuple[type] = (
     numpy.float_,
     numpy.float16,
     numpy.float32,
     numpy.float64,
-    numpy.float128,
+    numpy.longdouble,
 )
 
 NUMPY_INT_TYPES: Tuple[type] = (
     numpy.int_,
     numpy.int8,
     numpy.int16,
     numpy.int32,
```

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/data_types/spark_sql.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/data_types/spark_sql.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/default_dict.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/default_dict.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/fs.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/fs.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/iter.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/iter.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/log.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/log.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/namespace.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/s3.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/s3.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/h1st/utils/tools.py` & `h1st_contrib-2.1.8.dev1/h1st/utils/tools.py`

 * *Files identical despite different names*

### Comparing `h1st_contrib-2.1.2.dev0/pyproject.toml` & `h1st_contrib-2.1.8.dev1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "h1st-contrib"
-version = "2.1.2.dev0"
+version = "2.1.8.dev1"
 description = "Human-First AI (H1st)"
 authors = ["Aitomatic, Inc. <engineering@aitomatic.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://h1st.ai"
 repository = "https://github.com/h1st-ai/h1st"
 packages = [
-  { include = "h1st" },
+  {include = "h1st"},
+]
+include = [
+  "h1st/*",
 ]
-include = ["h1st/*"]
 
 
 [tool.poetry.dependencies]
 python = ">= 3.11"
 
 # Data Processing
 numpy = ">= 1.23"  # let higher dependencies figure
 pandas = ">= 1.5"  # let higher dependencies figure
 pyarrow = ">= 12.0.1"
-pyspark = ">= 3.4.0"
+pyspark = ">= 3.4.1"
 
 # Machine Learning / Deep Learning
 imbalanced-learn = ">= 0.10.1"
 scikit-fuzzy = ">= 0.4.2"
-scikit-learn = ">= 1.2.2"
-tensorflow = ">= 2.12.0"
-xgboost = ">= 1.7.5"
+scikit-learn = ">= 1.3.0"
+tensorflow = ">= 2.13.0"
+xgboost = ">= 1.7.6"
 
 # Trustworthy AI
 graphviz = ">= 0.20.1"
 lime = ">= 0.2.0.1"
 shap = {version = ">= 0.41.0", markers = "python_version < '3.11'"}
 
 # File Systems
@@ -45,18 +47,18 @@
 pyyaml = ">= 6.0"
 "ruamel.yaml" = ">= 0.17.21"
 tqdm = ">= 4.65.0"
 ulid-py = ">= 1.1.0"
 
 
 [tool.poetry.dev-dependencies]
-commitizen = ">= 3.3.0"
+commitizen = ">= 3.5.2"
 pre-commit = ">= 3.3.3"
 pylint = ">= 2.17.4"
-pytest = ">= 7.3.2"
+pytest = ">= 7.4.0"
 sphinx = ">= 7.0.1"
 sphinx-rtd-theme = ">= 1.2.2"
 
 
 [tool.poetry.scripts]
 h1st = 'h1st.utils.tools:h1st_cli'
```

### Comparing `h1st_contrib-2.1.2.dev0/PKG-INFO` & `h1st_contrib-2.1.8.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h1st-contrib
-Version: 2.1.2.dev0
+Version: 2.1.8.dev1
 Summary: Human-First AI (H1st)
 Home-page: https://h1st.ai
 License: Apache-2.0
 Author: Aitomatic, Inc.
 Author-email: engineering@aitomatic.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,26 +15,26 @@
 Requires-Dist: graphviz (>=0.20.1)
 Requires-Dist: imbalanced-learn (>=0.10.1)
 Requires-Dist: lime (>=0.2.0.1)
 Requires-Dist: loguru (>=0.7.0)
 Requires-Dist: numpy (>=1.23)
 Requires-Dist: pandas (>=1.5)
 Requires-Dist: pyarrow (>=12.0.1)
-Requires-Dist: pyspark (>=3.4.0)
+Requires-Dist: pyspark (>=3.4.1)
 Requires-Dist: python-dotenv (>=1.0.0)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: ruamel.yaml (>=0.17.21)
 Requires-Dist: s3fs (>=2023.6.0)
 Requires-Dist: scikit-fuzzy (>=0.4.2)
-Requires-Dist: scikit-learn (>=1.2.2)
+Requires-Dist: scikit-learn (>=1.3.0)
 Requires-Dist: shap (>=0.41.0) ; python_version < "3.11"
-Requires-Dist: tensorflow (>=2.12.0)
+Requires-Dist: tensorflow (>=2.13.0)
 Requires-Dist: tqdm (>=4.65.0)
 Requires-Dist: ulid-py (>=1.1.0)
-Requires-Dist: xgboost (>=1.7.5)
+Requires-Dist: xgboost (>=1.7.6)
 Project-URL: Repository, https://github.com/h1st-ai/h1st
 Description-Content-Type: text/markdown
 
 ## Join the Human-First AI revolution
 _“We humans have .. insight that can then be mixed with powerful AI .. to help move society forward. Second, we also have to build trust directly into our technology .. And third, all of the technology we build must be inclusive and respectful to everyone.”_
 <br/>— Satya Nadella, Microsoft CEO
```

