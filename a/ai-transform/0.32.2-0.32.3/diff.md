# Comparing `tmp/ai_transform-0.32.2.tar.gz` & `tmp/ai_transform-0.32.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.32.2.tar", last modified: Tue Jul 11 03:23:42 2023, max compression
+gzip compressed data, was "ai_transform-0.32.3.tar", last modified: Fri Jul 14 02:11:48 2023, max compression
```

## Comparing `ai_transform-0.32.2.tar` & `ai_transform-0.32.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.648690 ai_transform-0.32.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-11 03:23:26.000000 ai_transform-0.32.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 03:23:42.648690 ai_transform-0.32.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-11 03:23:26.000000 ai_transform-0.32.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.624689 ai_transform-0.32.2/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.628689 ai_transform-0.32.2/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.632689 ai_transform-0.32.2/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.632689 ai_transform-0.32.2/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.632689 ai_transform-0.32.2/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.636689 ai_transform-0.32.2/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.636689 ai_transform-0.32.2/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.636689 ai_transform-0.32.2/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-11 03:23:26.000000 ai_transform-0.32.2/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.628689 ai_transform-0.32.2/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 03:23:42.000000 ai_transform-0.32.2/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 03:23:26.000000 ai_transform-0.32.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 03:23:42.648690 ai_transform-0.32.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 03:23:26.000000 ai_transform-0.32.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.640689 ai_transform-0.32.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.640689 ai_transform-0.32.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.640689 ai_transform-0.32.2/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:42.644689 ai_transform-0.32.2/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 03:23:26.000000 ai_transform-0.32.2/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-14 02:11:28.000000 ai_transform-0.32.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 02:11:48.861410 ai_transform-0.32.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-14 02:11:28.000000 ai_transform-0.32.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29597 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 02:11:28.000000 ai_transform-0.32.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:11:48.861410 ai_transform-0.32.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-14 02:11:28.000000 ai_transform-0.32.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.32.2/LICENSE` & `ai_transform-0.32.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/README.md` & `ai_transform-0.32.3/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/__init__.py` & `ai_transform-0.32.3/ai_transform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.32.2"
+__version__ = "0.32.3"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.32.2/ai_transform/api/api.py` & `ai_transform-0.32.3/ai_transform/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,19 +406,22 @@
         response = self.post(suffix=f"/workflows/{job_id}/metadata", json=dict(metadata=metadata))
         return get_response(response)
 
     def _get_file_upload_urls(self, dataset_id: str, files: List[str]):
         response = self.post(suffix=f"/datasets/{dataset_id}/get_file_upload_urls", json=dict(files=files))
         return get_response(response)
 
-    def _get_temp_file_upload_url(self):
+    def _get_temp_file_upload_url(self, ext: str = None):
         """Use this for temporary file uploads.
         returns: {'download_url': ..., 'upload_url': ...}
         """
-        response = self.post(suffix=f"/services/get_temporary_file_upload_url")
+        body = {}
+        if ext is not None:
+            body["extension"] = ext
+        response = self.post(suffix=f"/services/get_temporary_file_upload_url", json=body)
         return get_response(response)
 
     def _upload_temporary_media(self, presigned_url: str, media_content: bytes):
         return requests.put(presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content)
 
     def _upload_media(self, presigned_url: str, media_content: bytes):
         # dont use get response since response cannot be json decoded
```

### Comparing `ai_transform-0.32.2/ai_transform/api/client.py` & `ai_transform-0.32.3/ai_transform/api/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import warnings
 
-from typing import Optional, Dict, Any
+from typing import Optional, Dict, Any, Union
 
 from ai_transform.api.api import API
 from ai_transform.api.helpers import process_token
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.types import Schema
 from ai_transform.errors import AuthException
 from ai_transform.constants import WELCOME_MESSAGE
@@ -76,23 +76,37 @@
             metadata=metadata,
             additional_information=additional_information,
             send_email=send_email,
             email=email,
             output=output,
         )
 
-    def insert_temp_local_media(self, file_path: str):
+    def insert_temp_local_media(self, file_path_or_bytes: Union[str, bytes], ext: str = None):
         """
         Insert temporary local media.
         """
-        data = self.api._get_temp_file_upload_url()
+        if isinstance(file_path_or_bytes, str):
+            with open(file_path_or_bytes, "rb") as fn_byte:
+                media_content = bytes(fn_byte.read())
+            if ext is None:
+                _, ext = os.path.splitext(file_path_or_bytes)
+                ext = ext[1:] # remove leading `.`
+            
+        elif isinstance(file_path_or_bytes, bytes):
+            media_content = file_path_or_bytes
+            if ext is None:
+                raise ValueError("Must set file ext i.e. `csv` or `png`")
+
+        else:
+            raise ValueError("`file_path_or_bytes` must be one of type `str` or `bytes`")
+
+        data = self.api._get_temp_file_upload_url(ext)
         upload_url = data["upload_url"]
         download_url = data["download_url"]
-        with open(file_path, "rb") as fn_byte:
-            media_content = bytes(fn_byte.read())
+            
         response = self.api._upload_temporary_media(presigned_url=upload_url, media_content=media_content)
         ic(response.content)
         return {"download_url": download_url}
 
     def list_project_keys(self):
         return self.api._list_project_keys()
```

### Comparing `ai_transform-0.32.2/ai_transform/api/helpers.py` & `ai_transform-0.32.3/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/api/wrappers.py` & `ai_transform-0.32.3/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/components/components.py` & `ai_transform-0.32.3/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/config.py` & `ai_transform-0.32.3/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/dataset/dataset.py` & `ai_transform-0.32.3/ai_transform/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,14 @@
         random_state: int = 0,
         is_random: bool = False,
         after_id: Optional[List] = None,
         worker_number: int = 0,
         max_retries: int = 3,
         retry_delay: int = 2,
     ) -> Dict[str, Any]:
-
         documents = []
         retry_count = 0
         while True:
             try:
                 chunk = self.get_documents(
                     page_size=page_size,
                     filters=filters,
```

### Comparing `ai_transform-0.32.2/ai_transform/dataset/field.py` & `ai_transform-0.32.3/ai_transform/dataset/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,14 @@
             accuracy=accuracy,
             cluster_ids=cluster_ids if cluster_ids is not None else [],
             dont_save_summaries=dont_save_summaries,
             filters=filters if filters is not None else [],
         )
 
     def create_centroid_documents(self):
-
         documents = self._dataset.get_all_documents(select_fields=[self._cluster_field, self._field])
         documents = documents["documents"]
 
         vectors = np.array([document[self._cluster_field] for document in documents])
 
         labels = [document[self._field] for document in documents]
```

### Comparing `ai_transform-0.32.2/ai_transform/engine/abstract_engine.py` & `ai_transform-0.32.3/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.32.3/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.32.3/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/engine/multipass_engine.py` & `ai_transform-0.32.3/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.32.3/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/engine/stable_engine.py` & `ai_transform-0.32.3/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/errors.py` & `ai_transform-0.32.3/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/logger.py` & `ai_transform-0.32.3/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/operator/abstract_operator.py` & `ai_transform-0.32.3/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/operator/dense_operator.py` & `ai_transform-0.32.3/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/timer.py` & `ai_transform-0.32.3/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/types.py` & `ai_transform-0.32.3/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/utils/document.py` & `ai_transform-0.32.3/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/utils/document_list.py` & `ai_transform-0.32.3/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/utils/example_documents.py` & `ai_transform-0.32.3/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/utils/json_encoder.py` & `ai_transform-0.32.3/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/utils/keyphrase.py` & `ai_transform-0.32.3/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.32.3/ai_transform/workflow/abstract_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         additional_information: str = "",
         send_email: bool = True,
         success_threshold: float = 0.8,
         email: dict = None,
         output: dict = None,
         **kwargs,  # TODO: Update workflows, This for deprecated arguments
     ):
-
         if job_id is None:
             job_id = str(uuid.uuid4())
             warnings.warn(f"No job id supplied, using {job_id}")
 
         self._name = name
         self._engine = engine
         self._job_id = job_id
```

### Comparing `ai_transform-0.32.2/ai_transform/workflow/context_manager.py` & `ai_transform-0.32.3/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform/workflow/helpers.py` & `ai_transform-0.32.3/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.32.3/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/setup.py` & `ai_transform-0.32.3/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/conftest.py` & `ai_transform-0.32.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_api/test_endpoints.py` & `ai_transform-0.32.3/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.32.3/tests/core/test_api/test_keyphrase.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import uuid
 
 from ai_transform.utils import List
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.api.client import Client
 from ai_transform.utils.keyphrase import Keyphrase
 
+
 # write a few tests
 class TestClient:
     def test_upsert_keyphrases(
         self, test_client: Client, test_keyphrase_dataset: Dataset, test_keyphrases: List[Keyphrase]
     ):
         # Test that upserting keyphrases is good
         field = "sample_1_label"
```

### Comparing `ai_transform-0.32.2/tests/core/test_api/test_wrappers.py` & `ai_transform-0.32.3/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.32.3/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_dataset/test_field.py` & `ai_transform-0.32.3/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.32.3/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.32.3/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_engine/test_engine.py` & `ai_transform-0.32.3/tests/core/test_engine/test_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ai_transform.utils.example_documents import mock_documents
 
 
 class TestAbstractEngine:
     def test_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
         class ExampleEngine(AbstractEngine):
             def apply(self) -> Any:
-
                 iterator = self.iterate()
                 for chunk in iterator:
                     new_batch = self.operator(chunk)
                     self.update_chunk(new_batch)
 
                 return
```

### Comparing `ai_transform-0.32.2/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.32.3/tests/core/test_engine/test_engine_playground.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from ai_transform.engine.stable_engine import StableEngine
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.utils import mock_documents
 
 
 class TestEnginePlayground:
     def test_engine_playground(self, full_dataset: Dataset, test_operator: AbstractOperator):
-
         engine = StableEngine(full_dataset, test_operator, documents=mock_documents(1000))
 
         assert engine.output_to_status
 
         engine()
 
         assert engine.output_documents
```

### Comparing `ai_transform-0.32.2/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.32.3/tests/core/test_engine/test_multipass_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 try:
     from sklearn.cluster import MiniBatchKMeans
 except:
     pass
 else:
-
     import time
     import numpy as np
 
     from ai_transform.dataset.dataset import Dataset
     from ai_transform.engine.multipass_engine import MultiPassEngine
 
     from ai_transform.operator.abstract_operator import AbstractOperator
```

### Comparing `ai_transform-0.32.2/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.32.3/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.32.3/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.32.3/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.32.3/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.2/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.32.3/tests/core/test_workflow/test_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,23 @@
         None,
         description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
     )
 
 
 class TestWorkflow:
     def test_workflow(self, test_paid_engine: AbstractEngine):
-
         workflow_name = "test_workflow"
         workflow = Workflow(name=workflow_name, engine=test_paid_engine, job_id="test_job1")
         res = workflow.run()
         assert res is None
 
         status = workflow.get_status()
         assert status["steps"][workflow_name]["n_processed_pricing"] == 20
 
     def test_workflow_no_refresh(self, test_paid_engine_no_refresh: AbstractEngine):
-
         workflow_name = "test_workflow"
         workflow = Workflow(name=workflow_name, engine=test_paid_engine_no_refresh, job_id="test_job2")
         res = workflow.run()
         assert res is None
 
         status = workflow.get_status()
         assert status["steps"][workflow_name]["n_processed_pricing"] == 20
@@ -66,15 +64,14 @@
         simple_workflow_dataset = test_client.Dataset("test-simple-workflow-dataset", expire=True)
         simple_workflow_dataset.insert_documents([{"_id": "0", "value": 0}])
 
         workflow_name = "Simple Workflow"
         time_sleep_value = 10
 
         with test_client.SimpleWorkflow(workflow_name=workflow_name, job_id="test-simple-workflow") as workflow:
-
             time.sleep(time_sleep_value)
             simple_workflow_dataset.update_documents([{"_id": "0", "value": 1}], ingest_in_background=False)
 
         status = workflow.get_status()
         assert status["status"] == "complete"
         assert status["steps"][workflow_name]["n_processed_pricing"] >= time_sleep_value
```

