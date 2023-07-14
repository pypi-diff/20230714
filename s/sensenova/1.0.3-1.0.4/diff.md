# Comparing `tmp/sensenova-1.0.3.tar.gz` & `tmp/sensenova-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sensenova-1.0.3.tar", last modified: Thu Jul 13 11:41:59 2023, max compression
+gzip compressed data, was "sensenova-1.0.4.tar", last modified: Fri Jul 14 06:17:04 2023, max compression
```

## Comparing `sensenova-1.0.3.tar` & `sensenova-1.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.3/LICENSE
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2337 2023-07-13 11:41:59.000000 sensenova-1.0.3/PKG-INFO
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2124 2023-07-11 10:58:41.000000 sensenova-1.0.3/README.md
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.3/pyproject.toml
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2010 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/_sensenova_scripts.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_requestor.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/api_resources/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/__init__.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/api_resources/abstract/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      790 2023-07-13 11:27:47.000000 sensenova-1.0.3/sensenova/api_resources/abstract/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/createable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/deletable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/downloadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/engine_api_resource.py
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      948 2023-07-13 11:26:18.000000 sensenova-1.0.3/sensenova/api_resources/abstract/file_deletable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/fileable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/listable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/abstract/uploadable_api_resource.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/dataset.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/error_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/fine_tune.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      559 2023-07-13 11:28:14.000000 sensenova-1.0.3/sensenova/api_resources/knowledge_base.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/model.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/api_resources/serving.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    17347 2023-07-13 11:34:42.000000 sensenova-1.0.3/sensenova/cli.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/error.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/object_classes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/sensenova_object.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/sensenova_response.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova/tests/
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/tests/__init__.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-07-12 10:50:35.000000 sensenova-1.0.3/sensenova/tests/test_chat_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4043 2023-07-13 03:17:07.000000 sensenova-1.0.3/sensenova/tests/test_datasets.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1171 2023-07-13 04:20:15.000000 sensenova-1.0.3/sensenova/tests/test_fine_tunes.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/tests/test_finetune_completion.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2191 2023-07-13 11:37:26.000000 sensenova-1.0.3/sensenova/tests/test_knowlege_bases.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      339 2023-07-13 04:39:51.000000 sensenova-1.0.3/sensenova/tests/test_models.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/tests/test_prepare_data.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      976 2023-07-13 04:25:50.000000 sensenova-1.0.3/sensenova/tests/test_servings.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.3/sensenova/upload_progress.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5770 2023-07-11 10:58:24.000000 sensenova-1.0.3/sensenova/util.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-07-13 02:46:13.000000 sensenova-1.0.3/sensenova/validators.py
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-13 11:38:41.000000 sensenova-1.0.3/sensenova/version.py
-drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-13 11:41:59.000000 sensenova-1.0.3/sensenova.egg-info/
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2337 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1789 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       64 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/entry_points.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       86 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-13 11:41:58.000000 sensenova-1.0.3/sensenova.egg-info/top_level.txt
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      631 2023-07-13 11:41:59.000000 sensenova-1.0.3/setup.cfg
--rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.3/setup.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-14 06:17:04.092750 sensenova-1.0.4/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1088 2023-06-29 07:22:18.000000 sensenova-1.0.4/LICENSE
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2331 2023-07-14 06:17:04.092750 sensenova-1.0.4/PKG-INFO
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2063 2023-07-14 05:26:58.000000 sensenova-1.0.4/README.md
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      244 2023-06-29 07:11:49.000000 sensenova-1.0.4/pyproject.toml
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-14 06:17:04.004750 sensenova-1.0.4/sensenova/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1179 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2055 2023-07-14 06:10:15.000000 sensenova-1.0.4/sensenova/_sensenova_scripts.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    15479 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_requestor.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-14 06:17:04.036750 sensenova-1.0.4/sensenova/api_resources/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      475 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/__init__.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-14 06:17:04.060750 sensenova-1.0.4/sensenova/api_resources/abstract/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      790 2023-07-13 11:27:47.000000 sensenova-1.0.4/sensenova/api_resources/abstract/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3053 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1691 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/createable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/deletable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2267 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/downloadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     3602 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      948 2023-07-13 11:26:18.000000 sensenova-1.0.4/sensenova/api_resources/abstract/file_deletable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1836 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/fileable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1833 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/listable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1861 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/abstract/uploadable_api_resource.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      768 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      504 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/dataset.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      569 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/error_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1208 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/fine_tune.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1116 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      559 2023-07-13 11:28:14.000000 sensenova-1.0.4/sensenova/api_resources/knowledge_base.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      177 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/model.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2133 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/api_resources/serving.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)    18120 2023-07-14 06:11:41.000000 sensenova-1.0.4/sensenova/cli.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2910 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/error.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      209 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/object_classes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     7143 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/sensenova_object.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      150 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/sensenova_response.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-14 06:17:04.092750 sensenova-1.0.4/sensenova/tests/
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/tests/__init__.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      844 2023-07-12 10:50:35.000000 sensenova-1.0.4/sensenova/tests/test_chat_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4043 2023-07-13 03:17:07.000000 sensenova-1.0.4/sensenova/tests/test_datasets.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1171 2023-07-13 04:20:15.000000 sensenova-1.0.4/sensenova/tests/test_fine_tunes.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      434 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/tests/test_finetune_completion.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2191 2023-07-13 11:37:26.000000 sensenova-1.0.4/sensenova/tests/test_knowlege_bases.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      339 2023-07-13 04:39:51.000000 sensenova-1.0.4/sensenova/tests/test_models.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     4097 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/tests/test_prepare_data.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      976 2023-07-13 04:25:50.000000 sensenova-1.0.4/sensenova/tests/test_servings.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1093 2023-06-29 07:11:49.000000 sensenova-1.0.4/sensenova/upload_progress.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     5897 2023-07-14 05:53:15.000000 sensenova-1.0.4/sensenova/util.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2840 2023-07-13 02:46:13.000000 sensenova-1.0.4/sensenova/validators.py
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       18 2023-07-14 06:02:25.000000 sensenova-1.0.4/sensenova/version.py
+drwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        0 2023-07-14 06:17:04.008750 sensenova-1.0.4/sensenova.egg-info/
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     2331 2023-07-14 06:17:03.000000 sensenova-1.0.4/sensenova.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)     1789 2023-07-14 06:17:03.000000 sensenova-1.0.4/sensenova.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)        1 2023-07-14 06:17:03.000000 sensenova-1.0.4/sensenova.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       65 2023-07-14 06:17:03.000000 sensenova-1.0.4/sensenova.egg-info/entry_points.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       86 2023-07-14 06:17:03.000000 sensenova-1.0.4/sensenova.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       10 2023-07-14 06:17:03.000000 sensenova-1.0.4/sensenova.egg-info/top_level.txt
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)      631 2023-07-14 06:17:04.092750 sensenova-1.0.4/setup.cfg
+-rwxr-xr-x   0 SENSETIME\wanzihao (840487773) SENSETIME\domain^users (840434177)       38 2023-06-29 07:11:49.000000 sensenova-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sensenova-1.0.3/LICENSE` & `sensenova-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/PKG-INFO` & `sensenova-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python client library for the Sensenova API
+Home-page: UNKNOWN
 Author: Sensetime
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sensenova Python Library
 
 The Sensenova Python library provides convenient access to the Sensenova API from applications written in the Python
@@ -17,19 +20,14 @@
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
 pip install --upgrade sensenova
 ```
 
-Install from source with:
-
-```sh
-python setup.py install
-```
 
 ## Usage
 
 ### Configure API KEY
 
 Set environment variable:
 
@@ -109,7 +107,8 @@
 ```sh
 sensenova tools fine_tunes.prepare_data -f data.json
 ```
 
 ## Requirements
 
 - Python 3.7.1+
+
```

### Comparing `sensenova-1.0.3/README.md` & `sensenova-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
 pip install --upgrade sensenova
 ```
 
-Install from source with:
-
-```sh
-python setup.py install
-```
 
 ## Usage
 
 ### Configure API KEY
 
 Set environment variable:
```

### Comparing `sensenova-1.0.3/sensenova/__init__.py` & `sensenova-1.0.4/sensenova/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/_sensenova_scripts.py` & `sensenova-1.0.4/sensenova/_sensenova_scripts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import logging
 
 import sys
 
 import sensenova
 from sensenova import version
-from sensenova.cli import tools_register, api_register
+from sensenova.cli import tools_register, api_register, display_error
 
 logger = logging.getLogger()
 formatter = logging.Formatter("[%(asctime)s] %(message)s")
 handler = logging.StreamHandler(sys.stderr)
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
@@ -58,16 +58,17 @@
     if args.secret_access_key is not None:
         sensenova.secret_access_key = args.secret_access_key
     if args.api_base is not None:
         sensenova.api_base = args.api_base
 
     try:
         args.func(args)
-    except Exception as e:
-        sys.stderr.write(str(e))
+    except sensenova.error.SensenovaError as e:
+        display_error(e)
+        return 1
     except KeyboardInterrupt:
         sys.stderr.write("\n")
         return 1
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `sensenova-1.0.3/sensenova/api_requestor.py` & `sensenova-1.0.4/sensenova/api_requestor.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/__init__.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/createable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/deletable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/downloadable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/downloadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/engine_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/file_deletable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/file_deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/fileable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/fileable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/listable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/abstract/uploadable_api_resource.py` & `sensenova-1.0.4/sensenova/api_resources/abstract/uploadable_api_resource.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/chat_completion.py` & `sensenova-1.0.4/sensenova/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/error_object.py` & `sensenova-1.0.4/sensenova/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/fine_tune.py` & `sensenova-1.0.4/sensenova/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/finetune_completion.py` & `sensenova-1.0.4/sensenova/api_resources/finetune_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/knowledge_base.py` & `sensenova-1.0.4/sensenova/api_resources/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/api_resources/serving.py` & `sensenova-1.0.4/sensenova/api_resources/serving.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/cli.py` & `sensenova-1.0.4/sensenova/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from argparse import ArgumentParser
 
 import sensenova.cli
-from sensenova.util import fine_tunes_hyperparams, finetune_completions_option_params
+from sensenova.util import fine_tunes_hyperparams, finetune_completions_option_params, fine_tune_lora_params
 from sensenova.validators import (
     apply_necessary_remediation,
     apply_processors,
     get_processors,
     read_any_format,
     write_out_file,
 )
@@ -238,23 +238,32 @@
     @classmethod
     def create(cls, args):
         create_args = {
             "model": args.model,
             "training_file": args.training_file,
             "suffix": args.suffix
         }
-        hyperparams = {}
+        training = {}
+        lora = {}
         params = fine_tunes_hyperparams()
+        lora_params = fine_tune_lora_params()
         for param in params:
             attr = getattr(args, param[0])
             if attr is not None:
                 if param[2]:
                     attr = eval(attr)
-                hyperparams[param[0]] = attr
-        create_args["hyperparams"] = hyperparams
+                if param in lora_params:
+                    lora[param[0]] = attr
+                else:
+                    training[param[0]] = attr
+        if len(lora.keys()) > 0:
+            training['lora'] = lora
+        create_args["hyperparams"] = {
+            "training": training
+        }
         resp = sensenova.FineTune.create(**create_args)
         print(resp)
 
     @classmethod
     def get(cls, args):
         resp = sensenova.FineTune.retrieve(id=args.id)
         print(resp)
@@ -582,7 +591,31 @@
     #     "--stream", help="Stream messages as they're ready.", action="store_true"
     # )
     #
     # for param in finetune_completions_option_params():
     #     opt.add_argument(f"--{param[0]}", help=param[1])
     #
     # sub.set_defaults(func=FinetuneCompletion.create)
+
+
+class bcolors:
+    HEADER = "\033[95m"
+    OKBLUE = "\033[94m"
+    OKGREEN = "\033[92m"
+    WARNING = "\033[93m"
+    FAIL = "\033[91m"
+    ENDC = "\033[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+
+
+def display_error(e):
+    extra = (
+        " (HTTP status code: {})".format(e.http_status)
+        if e.http_status is not None
+        else ""
+    )
+    sys.stderr.write(
+        "{}Error:{} {}{}\n".format(
+            bcolors.FAIL, bcolors.ENDC, e, extra
+        )
+    )
```

### Comparing `sensenova-1.0.3/sensenova/error.py` & `sensenova-1.0.4/sensenova/error.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/sensenova_object.py` & `sensenova-1.0.4/sensenova/sensenova_object.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/tests/test_chat_completion.py` & `sensenova-1.0.4/sensenova/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/tests/test_datasets.py` & `sensenova-1.0.4/sensenova/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/tests/test_fine_tunes.py` & `sensenova-1.0.4/sensenova/tests/test_fine_tunes.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/tests/test_knowlege_bases.py` & `sensenova-1.0.4/sensenova/tests/test_knowlege_bases.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/tests/test_prepare_data.py` & `sensenova-1.0.4/sensenova/tests/test_prepare_data.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/tests/test_servings.py` & `sensenova-1.0.4/sensenova/tests/test_servings.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/upload_progress.py` & `sensenova-1.0.4/sensenova/upload_progress.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova/util.py` & `sensenova-1.0.4/sensenova/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,26 @@
     ]
 
 
 def fine_tunes_hyperparams():
     # name, help, if eval
     return [
         ["max_steps", "The maximum number of training iterations.", True],
+        ["method", "The finetune method.", False],
         ["lr_scheduler_type", "Learning Rate Adjustment Strategy.", False],
         ["learning_rate", "Learning rate.", True],
         ["warmup_ratio", "Warmup iteration ratio.", True],
         ["weight_decay", "Regularized weight decay.", True],
         ["save_steps", "Weight saving iteration interval.", True],
         ["modules_to_save", "Modules that need to be trained and saved.", False],
+    ] + fine_tune_lora_params()
+
+
+def fine_tune_lora_params():
+    return [
         ["lora_rank", "The rank of the lora layer.", True],
         ["lora_dropout", "The dropout probability of the lora layer.", True],
         ["lora_alpha", "The regularization strength of the lora layer.", True]
     ]
 
 
 def logfmt(props):
```

### Comparing `sensenova-1.0.3/sensenova/validators.py` & `sensenova-1.0.4/sensenova/validators.py`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/sensenova.egg-info/PKG-INFO` & `sensenova-1.0.4/sensenova.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: sensenova
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python client library for the Sensenova API
+Home-page: UNKNOWN
 Author: Sensetime
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sensenova Python Library
 
 The Sensenova Python library provides convenient access to the Sensenova API from applications written in the Python
@@ -17,19 +20,14 @@
 You don't need this source code unless you want to modify the package. If you just
 want to use the package, just run:
 
 ```sh
 pip install --upgrade sensenova
 ```
 
-Install from source with:
-
-```sh
-python setup.py install
-```
 
 ## Usage
 
 ### Configure API KEY
 
 Set environment variable:
 
@@ -109,7 +107,8 @@
 ```sh
 sensenova tools fine_tunes.prepare_data -f data.json
 ```
 
 ## Requirements
 
 - Python 3.7.1+
+
```

### Comparing `sensenova-1.0.3/sensenova.egg-info/SOURCES.txt` & `sensenova-1.0.4/sensenova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sensenova-1.0.3/setup.cfg` & `sensenova-1.0.4/setup.cfg`

 * *Files identical despite different names*

