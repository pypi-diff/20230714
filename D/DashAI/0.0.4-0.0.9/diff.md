# Comparing `tmp/DashAI-0.0.4.tar.gz` & `tmp/DashAI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DashAI-0.0.4.tar", last modified: Wed Nov 23 15:39:24 2022, max compression
+gzip compressed data, was "DashAI-0.0.9.tar", last modified: Fri Jul 14 18:42:10 2023, max compression
```

## Comparing `DashAI-0.0.4.tar` & `DashAI-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,164 @@
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      712 2022-11-23 15:01:18.000000 DashAI-0.0.4/DashAI/__init__.py
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/back/
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/back/Models/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-22 21:12:33.000000 DashAI-0.0.4/DashAI/back/Models/__init__.py
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/back/Models/classes/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       21 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/classes/__init__.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1701 2022-11-17 23:47:29.000000 DashAI-0.0.4/DashAI/back/Models/classes/getters.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      605 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/Models/classes/knn.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      935 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/classes/model.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      111 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/classes/numericClassificationModel.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1645 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/Models/classes/numericalWrapperForText.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      438 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/Models/classes/randomForest.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      578 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/Models/classes/sklearnLikeModel.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      576 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/Models/classes/svm.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      105 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/classes/textClassificationModel.py
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/back/Models/enums/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-22 21:21:55.000000 DashAI-0.0.4/DashAI/back/Models/enums/__init__.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      125 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/enums/squema_types.py
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/back/Models/parameters/
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/back/Models/parameters/models_schemas/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1813 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/parameters/models_schemas/knn.json
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1624 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/parameters/models_schemas/numericalwrapperfortext.json
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3430 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/parameters/models_schemas/randomforest.json
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    10043 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/Models/parameters/models_schemas/svm.json
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/back/TaskLib/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-22 21:24:27.000000 DashAI-0.0.4/DashAI/back/TaskLib/__init__.py
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/back/TaskLib/task/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-22 21:23:05.000000 DashAI-0.0.4/DashAI/back/TaskLib/task/__init__.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      553 2022-11-17 23:47:20.000000 DashAI-0.0.4/DashAI/back/TaskLib/task/numericClassificationTask.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5177 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/TaskLib/task/taskMain.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      889 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/TaskLib/task/taskMetaclass.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      775 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/TaskLib/task/textClassificationTask.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-22 21:12:26.000000 DashAI-0.0.4/DashAI/back/__init__.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      504 2022-11-17 23:47:18.000000 DashAI-0.0.4/DashAI/back/configObject.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      267 2022-11-22 20:34:46.000000 DashAI-0.0.4/DashAI/back/db.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1846 2022-11-17 18:07:33.000000 DashAI-0.0.4/DashAI/back/generate_dataset.py
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4082 2022-11-23 14:24:33.000000 DashAI-0.0.4/DashAI/back/main.py
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/front/
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/front/build/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      715 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/asset-manifest.json
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    15406 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/favicon.ico
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/front/build/images/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6761 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/images/loaded.png
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6708 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/images/loading.png
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    95587 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/images/logo.png
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      641 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/index.html
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5347 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/logo192.png
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     9664 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/logo512.png
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      492 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/manifest.json
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       67 2022-11-22 20:54:30.000000 DashAI-0.0.4/DashAI/front/build/robots.txt
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI/front/build/static/
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/front/build/static/css/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)   199665 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/css/main.8b939f52.css
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)   483162 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/css/main.8b939f52.css.map
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/front/build/static/js/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4611 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    10592 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js.map
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)   400863 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/js/main.4b04b4b2.js
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1944 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/js/main.4b04b4b2.js.LICENSE.txt
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)  1542542 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/js/main.4b04b4b2.js.map
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.122284 DashAI-0.0.4/DashAI/front/build/static/media/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    78220 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/media/Quicksand-Bold.a0a11318dd0b528da77d.ttf
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    78628 2022-11-22 20:54:41.000000 DashAI-0.0.4/DashAI/front/build/static/media/Quicksand-Regular.04b11c8f0d4d58c1bed1.ttf
-drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2022-11-23 15:39:24.118284 DashAI-0.0.4/DashAI.egg-info/
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1257 2022-11-23 15:39:24.000000 DashAI-0.0.4/DashAI.egg-info/PKG-INFO
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2212 2022-11-23 15:39:24.000000 DashAI-0.0.4/DashAI.egg-info/SOURCES.txt
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        1 2022-11-23 15:39:24.000000 DashAI-0.0.4/DashAI.egg-info/dependency_links.txt
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       37 2022-11-23 15:39:24.000000 DashAI-0.0.4/DashAI.egg-info/requires.txt
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        7 2022-11-23 15:39:24.000000 DashAI-0.0.4/DashAI.egg-info/top_level.txt
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       88 2022-11-23 15:34:01.000000 DashAI-0.0.4/MANIFEST.in
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1257 2022-11-23 15:39:24.122284 DashAI-0.0.4/PKG-INFO
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      792 2022-11-23 14:57:07.000000 DashAI-0.0.4/README.md
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       92 2022-11-23 15:24:09.000000 DashAI-0.0.4/dashai
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       38 2022-11-23 15:39:24.122284 DashAI-0.0.4/setup.cfg
--rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      854 2022-11-23 15:39:07.000000 DashAI-0.0.4/setup.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      894 2023-05-12 14:21:06.000000 DashAI-0.0.9/DashAI/__init__.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-01-06 17:26:35.000000 DashAI-0.0.9/DashAI/back/__init__.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/api/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-14 14:16:58.000000 DashAI-0.0.9/DashAI/back/api/__init__.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/api/api_v0/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-14 14:16:58.000000 DashAI-0.0.9/DashAI/back/api/api_v0/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      170 2023-03-14 14:16:58.000000 DashAI-0.0.9/DashAI/back/api/api_v0/api.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/api/api_v0/endpoints/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-14 14:16:58.000000 DashAI-0.0.9/DashAI/back/api/api_v0/endpoints/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2321 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/api_v0/endpoints/old_endpoints.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      325 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/api_v0/endpoints/session_class.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/api/api_v1/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-14 14:16:58.000000 DashAI-0.0.9/DashAI/back/api/api_v1/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      502 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/api_v1/api.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-14 14:16:58.000000 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     7360 2023-07-14 17:43:46.000000 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/components.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     9150 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/datasets.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4953 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/experiments.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2619 2023-07-14 18:37:32.000000 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/runner.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6944 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/api_v1/endpoints/runs.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      208 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/api/deps.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      697 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/config_object.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/core/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-28 21:28:16.000000 DashAI-0.0.9/DashAI/back/core/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1199 2023-07-14 14:29:55.000000 DashAI-0.0.9/DashAI/back/core/config.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/core/enums/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-10 14:23:45.000000 DashAI-0.0.9/DashAI/back/core/enums/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      175 2023-03-10 14:23:45.000000 DashAI-0.0.9/DashAI/back/core/enums/squema_types.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      269 2023-06-30 14:13:39.000000 DashAI-0.0.9/DashAI/back/core/enums/status.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3204 2023-07-14 18:37:32.000000 DashAI-0.0.9/DashAI/back/core/runner.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/database/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-01 13:18:44.000000 DashAI-0.0.9/DashAI/back/database/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3948 2023-06-30 14:13:39.000000 DashAI-0.0.9/DashAI/back/database/models.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      221 2023-03-28 21:28:16.000000 DashAI-0.0.9/DashAI/back/database/session.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/dataloaders/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      468 2023-05-12 14:20:59.000000 DashAI-0.0.9/DashAI/back/dataloaders/__init__.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/back/dataloaders/classes/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-01 13:18:44.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2521 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/audio_dataloader.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3218 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/csv_dataloader.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6833 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/dashai_dataset.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     7967 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/dataloader.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1503 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/dataloader_params.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2552 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/image_dataloader.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3214 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/json_dataloader.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4567 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/dataloaders/classes/tabular_dataloader.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1175 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/main.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/metrics/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      316 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/metrics/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      128 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/metrics/base_metric.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/metrics/classification/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/metrics/classification/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1149 2023-07-14 18:24:31.000000 DashAI-0.0.9/DashAI/back/metrics/classification/accuracy.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1302 2023-07-14 18:20:31.000000 DashAI-0.0.9/DashAI/back/metrics/classification/f1.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1345 2023-07-14 18:24:03.000000 DashAI-0.0.9/DashAI/back/metrics/classification/precision.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1324 2023-07-07 14:35:50.000000 DashAI-0.0.9/DashAI/back/metrics/classification/recall.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1564 2023-07-07 14:35:50.000000 DashAI-0.0.9/DashAI/back/metrics/classification_metric.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/models/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      388 2023-04-12 21:39:39.000000 DashAI-0.0.9/DashAI/back/models/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1231 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/base_model.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/models/classes/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       21 2023-03-01 13:18:44.000000 DashAI-0.0.9/DashAI/back/models/classes/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1663 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/classes/getters.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1452 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/classes/numerical_wrapper_for_text.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5886 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/classes/tc_transformer_eng_spa.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/models/hugging_face/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-06-30 14:13:43.000000 DashAI-0.0.9/DashAI/back/models/hugging_face/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5334 2023-07-07 14:35:50.000000 DashAI-0.0.9/DashAI/back/models/hugging_face/distilbert_transformer.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/models/scikit_learn/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-28 21:28:16.000000 DashAI-0.0.9/DashAI/back/models/scikit_learn/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      441 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/scikit_learn/k_neighbors_classifier.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      436 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/scikit_learn/random_forest_classifier.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1374 2023-07-07 14:35:50.000000 DashAI-0.0.9/DashAI/back/models/scikit_learn/sklearn_like_model.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      471 2023-07-14 15:53:03.000000 DashAI-0.0.9/DashAI/back/models/scikit_learn/svc.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      161 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/tabular_classification_model.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      152 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/text_classification_model.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       69 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/models/translation_model.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/registries/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       86 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/registries/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    14125 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/registries/component_registry.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3624 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/registries/relationship_manager.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/back/tasks/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      289 2023-03-13 17:47:01.000000 DashAI-0.0.9/DashAI/back/tasks/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3093 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/tasks/base_task.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1482 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/tasks/tabular_classification_task.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1390 2023-06-30 14:13:43.000000 DashAI-0.0.9/DashAI/back/tasks/text_classification_task.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      855 2023-06-14 18:48:34.000000 DashAI-0.0.9/DashAI/back/tasks/translation_task.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/front/
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/front/build/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      713 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/asset-manifest.json
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    15406 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/favicon.ico
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/front/build/images/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1719 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/back.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      295 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/close.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      607 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/cog-f.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6761 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/loaded.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6708 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/loading.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    95587 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/logo.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1162 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/search.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1004 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/settings.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      441 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/images/trash.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      641 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/index.html
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/front/build/info_images/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    13620 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/info_images/csv_files.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    16554 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/info_images/image_files.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    13627 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/info_images/json_files.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)   571355 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/info_images/json_format.svg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5347 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/logo192.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     9664 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/logo512.png
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      492 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/manifest.json
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       67 2023-07-14 15:53:17.000000 DashAI-0.0.9/DashAI/front/build/robots.txt
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI/front/build/static/
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.994515 DashAI-0.0.9/DashAI/front/build/static/css/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1189 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/css/main.715072ae.css
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1772 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/css/main.715072ae.css.map
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/DashAI/front/build/static/js/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4611 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    10592 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js.map
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)  1117239 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/js/main.f87b2cdc.js
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2658 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/js/main.f87b2cdc.js.LICENSE.txt
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)  5021749 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/js/main.f87b2cdc.js.map
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/DashAI/front/build/static/media/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    31988 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/media/Quicksand-Bold.9418150e286e7a45cdf5.woff2
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    78220 2023-07-14 15:53:46.000000 DashAI-0.0.9/DashAI/front/build/static/media/Quicksand-Bold.a0a11318dd0b528da77d.ttf
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.990515 DashAI-0.0.9/DashAI.egg-info/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5133 2023-07-14 18:42:09.000000 DashAI-0.0.9/DashAI.egg-info/PKG-INFO
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4886 2023-07-14 18:42:09.000000 DashAI-0.0.9/DashAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        1 2023-07-14 18:42:09.000000 DashAI-0.0.9/DashAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       38 2023-07-14 18:42:09.000000 DashAI-0.0.9/DashAI.egg-info/entry_points.txt
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      275 2023-07-14 18:42:09.000000 DashAI-0.0.9/DashAI.egg-info/requires.txt
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       13 2023-07-14 18:42:09.000000 DashAI-0.0.9/DashAI.egg-info/top_level.txt
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       89 2023-05-12 14:21:06.000000 DashAI-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5133 2023-07-14 18:42:09.998515 DashAI-0.0.9/PKG-INFO
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4356 2023-05-12 14:21:06.000000 DashAI-0.0.9/README.rst
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1225 2023-06-14 18:48:34.000000 DashAI-0.0.9/pyproject.toml
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)       38 2023-07-14 18:42:09.998515 DashAI-0.0.9/setup.cfg
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2184 2023-07-14 18:00:49.000000 DashAI-0.0.9/setup.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/tests/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-01 13:18:44.000000 DashAI-0.0.9/tests/__init__.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/tests/back/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-01 13:18:44.000000 DashAI-0.0.9/tests/back/__init__.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/tests/back/api/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-28 21:28:16.000000 DashAI-0.0.9/tests/back/api/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    19965 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/api/test_components_api.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4263 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/api/test_datasets.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     3563 2023-05-12 14:21:06.000000 DashAI-0.0.9/tests/back/api/test_experiments.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     6585 2023-07-14 15:53:03.000000 DashAI-0.0.9/tests/back/api/test_runner.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4935 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/api/test_runs.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     1381 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/conftest.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/tests/back/metrics/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/metrics/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     4302 2023-07-07 14:35:50.000000 DashAI-0.0.9/tests/back/metrics/test_classification_metrics.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/tests/back/registries/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-03-13 17:47:01.000000 DashAI-0.0.9/tests/back/registries/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)    14376 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/registries/test_registry.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     2011 2023-06-14 18:48:34.000000 DashAI-0.0.9/tests/back/registries/test_relationship_manager.py
+drwxrwxr-x   0 ctamblay  (1000) ctamblay  (1000)        0 2023-07-14 18:42:09.998515 DashAI-0.0.9/tests/back/tasks/
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)        0 2023-06-05 21:06:17.000000 DashAI-0.0.9/tests/back/tasks/__init__.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)     5102 2023-06-30 14:13:43.000000 DashAI-0.0.9/tests/back/tasks/test_tasks.py
+-rw-rw-r--   0 ctamblay  (1000) ctamblay  (1000)      199 2023-03-14 14:16:58.000000 DashAI-0.0.9/tests/back/test_main.py
```

### Comparing `DashAI-0.0.4/DashAI/back/Models/classes/getters.py` & `DashAI-0.0.9/DashAI/back/models/classes/getters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 from importlib import import_module
 from inspect import isclass
 from pathlib import Path
 from pkgutil import iter_modules
 
-from Models.classes import base_path
+from DashAI.back.models.classes import base_path
 
 
 def introspect_classes():
     classes_dict = {}
-
     # iterate through the modules in the current package
     package_dir = Path(__file__).resolve().parent
-    for (_, module_name, _) in iter_modules([str(package_dir)]):
+    for _, module_name, _ in iter_modules([str(package_dir)]):
         # import the module and iterate through its attributes
         module = import_module(f"{base_path}.{module_name}")
         for attribute_name in dir(module):
             attribute = getattr(module, attribute_name)
 
             if isclass(attribute):
                 # Add the class to this package's variables
                 class_name = attribute.__name__
                 if class_name not in classes_dict.keys():
                     classes_dict[class_name] = attribute
-
     return classes_dict
 
 
 def filter_by_parent(parent_class_name):
     class_dict = introspect_classes()
     parent_class = class_dict[parent_class_name]
     filtered_dict = {}
-
-    for class_name in class_dict.keys():
+    for class_name in class_dict:
         if (
             issubclass(class_dict[class_name], parent_class)
             and parent_class_name != class_name
         ):
             filtered_dict[class_name] = class_dict[class_name]
-
     return filtered_dict
 
 
 def get_model_params_from_task(task_name):
-    """
-    It returns a dictionary with a list of the available models for the
-    task or an error if the squema
-    """
+    """Return a dictionary with a list of the available models for the task."""
+    model_class_name = f"{task_name[:-4]}Model"
     try:
-        model_class_name = f"{task_name[:-4]}Model"
         dict = filter_by_parent(model_class_name)
         return {"models": list(dict.keys())}
-    except:
+    except TypeError:
         return {"error": f"{model_class_name} not found"}
```

### Comparing `DashAI-0.0.4/DashAI/back/Models/classes/numericalWrapperForText.py` & `DashAI-0.0.9/DashAI/back/models/classes/numerical_wrapper_for_text.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import json
+
 from sklearn.feature_extraction.text import CountVectorizer
-from Models.classes.sklearnLikeModel import SkleanLikeModel
-from Models.classes.textClassificationModel import TextClassificationModel
+
+from DashAI.back.models import SklearnLikeModel
+from DashAI.back.models.text_classification_model import TextClassificationModel
 
 
-class NumericalWrapperForText(SkleanLikeModel, TextClassificationModel):
-    """
-    Wrapper for TextClassificationTask that uses a numericClassificationModel 
-    to classify text, it uses a simple bag of words model to vectorize the 
-    text and give it to the numerical model to perform the prediction.
-    """
+class NumericalWrapperForText(TextClassificationModel, SklearnLikeModel):
+    """Text classification metamodel."""
 
     MODEL = "numericalwrapperfortext"
-    with open(f"Models/parameters/models_schemas/{MODEL}.json") as f:
+    with open(f"DashAI/back/models/parameters/models_schemas/{MODEL}.json") as f:
         SCHEMA = json.load(f)
 
     def __init__(self, **kwargs) -> None:
         ngram_min_n = kwargs.pop("ngram_min_n")
         ngram_max_n = kwargs.pop("ngram_max_n")
-        kwargs["ngram_range"] = (ngram_min_n,ngram_max_n)
+        kwargs["ngram_range"] = (ngram_min_n, ngram_max_n)
         self.classifier = kwargs.pop("numeric_classifier")
         self.vectorizer = CountVectorizer(**kwargs)
 
     def fit(self, x, y):
         self.classifier.fit(self.vectorizer.fit_transform(x), y)
 
     def predict(self, x):
         return self.classifier.predict(self.vectorizer.transform(x))
-    
+
     def score(self, x, y):
         return self.classifier.score(self.vectorizer.transform(x), y)
 
     def get_params(self):
         ngram_min, ngram_max = self.vectorizer.get_params()["ngram_range"]
         params_dict = {
             "numeric_classifier": {
                 "choice": self.classifier.MODEL,
-                **self.classifier.get_params()
+                **self.classifier.get_params(),
             },
             "ngram_min_n": ngram_min,
             "ngram_max_n": ngram_max,
         }
-        return params_dict
+        return params_dict
```

### Comparing `DashAI-0.0.4/DashAI/front/build/favicon.ico` & `DashAI-0.0.9/DashAI/front/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/images/loaded.png` & `DashAI-0.0.9/DashAI/front/build/images/loaded.png`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/images/loading.png` & `DashAI-0.0.9/DashAI/front/build/images/loading.png`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/images/logo.png` & `DashAI-0.0.9/DashAI/front/build/images/logo.png`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/index.html` & `DashAI-0.0.9/DashAI/front/build/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>DashAI</title><script defer="defer" src="/static/js/main.4b04b4b2.js"></script><link href="/static/css/main.8b939f52.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>DashAI</title><script defer="defer" src="/static/js/main.f87b2cdc.js"></script><link href="/static/css/main.715072ae.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `DashAI-0.0.4/DashAI/front/build/logo192.png` & `DashAI-0.0.9/DashAI/front/build/logo192.png`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/logo512.png` & `DashAI-0.0.9/DashAI/front/build/logo512.png`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js` & `DashAI-0.0.9/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js`

 * *Files identical despite different names*

### Comparing `DashAI-0.0.4/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js.map` & `DashAI-0.0.9/DashAI/front/build/static/js/787.6b0bb1a2.chunk.js.map`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'mappings'": "'mRAAA,IAAIA,EAAEC,EAAEC,EAAEC,EAAEC,EAAE,SAASJ,EAAEC,GAAG,MAAM,CAACI,KAAKL,EAAEM,WAAM,IAASL,GAAG,EAAEA,EAAEM,MAAM,EAAEC,QAAQ,GAAGC,GAAG,MAAMC,OAAOC,KAAKC,MAAM,KAAKF,OAAOG,KAAKC,MAAM,cAAcD,KAAKE,UAAU,MAAM,EAAEC,EAAE,SAAShB,EAAEC,GAAG,IAAI,GAAGgB,oBAAoBC,oBAAoBC,SAASnB,GAAG,CAAC,GAAG,gBAAgBA,KAAK,2BAA2BoB,MAAM,OAAO,IAAIlB,EAAE,IAAIe,qBAAqB,SAASjB,GAAG,OAAOA,EAAEqB,aAAaC,IAAIrB,EAAE,IAAI,OAAOC,EAAEqB,QAAQ,CAACC,KAAKxB,EAAEyB,UAAS,IAAKvB,CAAC,CAAC,CAAC,MAAMF,GAAG,CAAC,EAAE0B,EAAE,SAAS1B,EAAEC,G […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "static/js/787.6b0bb1a2.chunk.js",
-    "mappings": "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",
+    "mappings": "mRAAA,IAAIA,EAAEC,EAAEC,EAAEC,EAAEC,EAAE,SAASJ,EAAEC,GAAG,MAAM,CAACI,KAAKL,EAAEM,WAAM,IAASL,GAAG,EAAEA,EAAEM,MAAM,EAAEC,QAAQ,GAAGC,GAAG,MAAMC,OAAOC,KAAKC,MAAM,KAAKF,OAAOG,KAAKC,MAAM,cAAcD,KAAKE,UAAU,MAAM,EAAEC,EAAE,SAAShB,EAAEC,GAAG,IAAI,GAAGgB,oBAAoBC,oBAAoBC,SAASnB,GAAG,CAAC,GAAG,gBAAgBA,KAAK,2BAA2BoB,MAAM,OAAO,IAAIlB,EAAE,IAAIe,qBAAqB,SAASjB,GAAG,OAAOA,EAAEqB,aAAaC,IAAIrB,EAAE,IAAI,OAAOC,EAAEqB,QAAQ,CAACC,KAAKxB,EAAEyB,UAAS,IAAKvB,CAAC,CAAC,CAAC,MAAMF,GAAG,CAAC,EAAE0B,EAAE,SAAS1B,EAAEC,GAAG,IAAIC,EAAE,SAASA,EAAEC,GAAG,aAAaA,EAAEqB,MAAM,WAAWG,SAASC,kBAAkB5B,EAAEG,GAAGF,IAAI4B,oBAAoB,mBAAmB3B,GAAE,GAAI2B,oBAAoB,WAAW3B,GAAE,IAAK,EAAE4B,iBAAiB,mBAAmB5B,GAAE,GAAI4B,iBAAiB,WAAW5B,GAAE,EAAG,EAAE6B,EAAE,SAAS/B,GAAG8B,iBAAiB,YAAY,SAAS7B,GAAGA,EAAE+B,WAAWhC,EAAEC,EAAE,IAAG,EAAG,EAAEgC,EAAE,SAASjC,EAAEC,EAAEC,GAAG,IAAIC,EAAE,OAAO,SAASC,GAAGH,EAAEK,OAAO,IAAIF,GAAGF,KAAKD,EAAEM,MAAMN,EAAEK,OAAOH,GAAG,IAAIF,EAAEM,YAAO,IAASJ,KAAKA,EAAEF,EAAEK,MAAMN,EAAEC,IAAI,CAAC,EAAEiC,GAAG,EAAEC,EAAE,WAAW,MAAM,WAAWR,SAASC,gBAAgB,EAAE,GAAG,EAAEQ,EAAE,WAAWV,GAAG,SAAS1B,GAAG,IAAIC,EAAED,EAAEqC,UAAUH,EAAEjC,CAAC,IAAG,EAAG,EAAEqC,EAAE,WAAW,OAAOJ,EAAE,IAAIA,EAAEC,IAAIC,IAAIL,GAAG,WAAWQ,YAAY,WAAWL,EAAEC,IAAIC,GAAG,GAAG,EAAE,KAAK,CAAKI,sBAAkB,OAAON,CAAC,EAAE,EAAEO,EAAE,SAASzC,EAAEC,GAAG,IAAIC,EAAEC,EAAEmC,IAAIZ,EAAEtB,EAAE,OAAO8B,EAAE,SAASlC,GAAG,2BAA2BA,EAAEK,OAAO+B,GAAGA,EAAEM,aAAa1C,EAAE2C,UAAUxC,EAAEqC,kBAAkBd,EAAEpB,MAAMN,EAAE2C,UAAUjB,EAAElB,QAAQoC,KAAK5C,GAAGE,GAAE,IAAK,EAAEiC,EAAEU,OAAOC,aAAaA,YAAYC,kBAAkBD,YAAYC,iBAAiB,0BAA0B,GAAGX,EAAED,EAAE,KAAKnB,EAAE,QAAQkB,IAAIC,GAAGC,KAAKlC,EAAE+B,EAAEjC,EAAE0B,EAAEzB,GAAGkC,GAAGD,EAAEC,GAAGJ,GAAG,SAAS5B,GAAGuB,EAAEtB,EAAE,OAAOF,EAAE+B,EAAEjC,EAAE0B,EAAEzB,GAAG+C,uBAAuB,WAAWA,uBAAuB,WAAWtB,EAAEpB,MAAMwC,YAAYlC,MAAMT,EAAEkC,UAAUnC,GAAE,EAAG,GAAG,GAAG,IAAI,EAAE+C,GAAE,EAAGC,GAAG,EAAEC,EAAE,SAASnD,EAAEC,GAAGgD,IAAIR,GAAG,SAASzC,GAAGkD,EAAElD,EAAEM,KAAK,IAAI2C,GAAE,GAAI,IAAI/C,EAAEC,EAAE,SAASF,GAAGiD,GAAG,GAAGlD,EAAEC,EAAE,EAAEiC,EAAE9B,EAAE,MAAM,GAAG+B,EAAE,EAAEC,EAAE,GAAGE,EAAE,SAAStC,GAAG,IAAIA,EAAEoD,eAAe,CAAC,IAAInD,EAAEmC,EAAE,GAAGjC,EAAEiC,EAAEA,EAAEiB,OAAO,GAAGlB,GAAGnC,EAAE2C,UAAUxC,EAAEwC,UAAU,KAAK3C,EAAE2C,UAAU1C,EAAE0C,UAAU,KAAKR,GAAGnC,EAAEM,MAAM8B,EAAEQ,KAAK5C,KAAKmC,EAAEnC,EAAEM,MAAM8B,EAAE,CAACpC,IAAImC,EAAED,EAAE5B,QAAQ4B,EAAE5B,MAAM6B,EAAED,EAAE1B,QAAQ4B,EAAElC,IAAI,CAAC,EAAEiD,EAAEnC,EAAE,eAAesB,GAAGa,IAAIjD,EAAE+B,EAAE9B,EAAE+B,EAAEjC,GAAGyB,GAAG,WAAWyB,EAAEG,cAAchC,IAAIgB,GAAGpC,GAAE,EAAG,IAAI6B,GAAG,WAAWI,EAAE,EAAEe,GAAG,EAAEhB,EAAE9B,EAAE,MAAM,GAAGF,EAAE+B,EAAE9B,EAAE+B,EAAEjC,EAAE,IAAI,EAAEsD,EAAE,CAACC,SAAQ,EAAGC,SAAQ,GAAIC,EAAE,IAAI/C,KAAKgD,EAAE,SAASxD,EAAEC,GAAGJ,IAAIA,EAAEI,EAAEH,EAAEE,EAAED,EAAE,IAAIS,KAAKiD,EAAE/B,qBAAqBgC,IAAI,EAAEA,EAAE,WAAW,GAAG5D,GAAG,GAAGA,EAAEC,EAAEwD,EAAE,CAAC,IAAItD,EAAE,CAAC0D,UAAU,cAAczD,KAAKL,EAAEwB,KAAKuC,OAAO/D,EAAE+D,OAAOC,WAAWhE,EAAEgE,WAAWrB,UAAU3C,EAAEqC,UAAU4B,gBAAgBjE,EAAEqC,UAAUpC,GAAGE,EAAE+D,SAAS,SAASlE,GAAGA,EAAEI,EAAE,IAAID,EAAE,EAAE,CAAC,EAAEgE,EAAE,SAASnE,GAAG,GAAGA,EAAEgE,WAAW,CAAC,IAAI/D,GAAGD,EAAEqC,UAAU,KAAK,IAAI1B,KAAKmC,YAAYlC,OAAOZ,EAAEqC,UAAU,eAAerC,EAAEwB,KAAK,SAASxB,EAAEC,GAAG,IAAIC,EAAE,WAAWyD,EAAE3D,EAAEC,GAAGG,GAAG,EAAED,EAAE,WAAWC,GAAG,EAAEA,EAAE,WAAWyB,oBAAoB,YAAY3B,EAAEqD,GAAG1B,oBAAoB,gBAAgB1B,EAAEoD,EAAE,EAAEzB,iBAAiB,YAAY5B,EAAEqD,GAAGzB,iBAAiB,gBAAgB3B,EAAEoD,EAAE,CAAhO,CAAkOtD,EAAED,GAAG2D,EAAE1D,EAAED,EAAE,CAAC,EAAE4D,EAAE,SAAS5D,GAAG,CAAC,YAAY,UAAU,aAAa,eAAekE,SAAS,SAASjE,GAAG,OAAOD,EAAEC,EAAEkE,EAAEZ,EAAE,GAAG,EAAEa,EAAE,SAASlE,EAAEgC,GAAG,IAAIC,EAAEC,EAAEE,IAAIG,EAAErC,EAAE,OAAO6C,EAAE,SAASjD,GAAGA,EAAE2C,UAAUP,EAAEI,kBAAkBC,EAAEnC,MAAMN,EAAEiE,gBAAgBjE,EAAE2C,UAAUF,EAAEjC,QAAQoC,KAAK5C,GAAGmC,GAAE,GAAI,EAAEe,EAAElC,EAAE,cAAciC,GAAGd,EAAEF,EAAE/B,EAAEuC,EAAEP,GAAGgB,GAAGxB,GAAG,WAAWwB,EAAEI,cAAchC,IAAI2B,GAAGC,EAAER,YAAY,IAAG,GAAIQ,GAAGnB,GAAG,WAAW,IAAIf,EAAEyB,EAAErC,EAAE,OAAO+B,EAAEF,EAAE/B,EAAEuC,EAAEP,GAAG/B,EAAE,GAAGF,GAAG,EAAED,EAAE,KAAK4D,EAAE9B,kBAAkBd,EAAEiC,EAAE9C,EAAEyC,KAAK5B,GAAG6C,GAAG,GAAG,EAAEQ,EAAE,CAAC,EAAEC,EAAE,SAAStE,EAAEC,GAAG,IAAIC,EAAEC,EAAEmC,IAAIJ,EAAE9B,EAAE,OAAO+B,EAAE,SAASnC,GAAG,IAAIC,EAAED,EAAE2C,UAAU1C,EAAEE,EAAEqC,kBAAkBN,EAAE5B,MAAML,EAAEiC,EAAE1B,QAAQoC,KAAK5C,GAAGE,IAAI,EAAEkC,EAAEpB,EAAE,2BAA2BmB,GAAG,GAAGC,EAAE,CAAClC,EAAE+B,EAAEjC,EAAEkC,EAAEjC,GAAG,IAAIwC,EAAE,WAAW4B,EAAEnC,EAAEzB,MAAM2B,EAAEkB,cAAchC,IAAIa,GAAGC,EAAEM,aAAa2B,EAAEnC,EAAEzB,KAAI,EAAGP,GAAE,GAAI,EAAE,CAAC,UAAU,SAASgE,SAAS,SAASlE,GAAG8B,iBAAiB9B,EAAEyC,EAAE,CAAC8B,MAAK,EAAGd,SAAQ,GAAI,IAAI/B,EAAEe,GAAE,GAAIV,GAAG,SAAS5B,GAAG+B,EAAE9B,EAAE,OAAOF,EAAE+B,EAAEjC,EAAEkC,EAAEjC,GAAG+C,uBAAuB,WAAWA,uBAAuB,WAAWd,EAAE5B,MAAMwC,YAAYlC,MAAMT,EAAEkC,UAAUgC,EAAEnC,EAAEzB,KAAI,EAAGP,GAAE,EAAG,GAAG,GAAG,GAAG,CAAC,EAAEsE,EAAE,SAASxE,GAAG,IAAIC,EAAEC,EAAEE,EAAE,QAAQH,EAAE,WAAW,IAAI,IAAIA,EAAE6C,YAAY2B,iBAAiB,cAAc,IAAI,WAAW,IAAIzE,EAAE8C,YAAY4B,OAAOzE,EAAE,CAAC6D,UAAU,aAAanB,UAAU,GAAG,IAAI,IAAIzC,KAAKF,EAAE,oBAAoBE,GAAG,WAAWA,IAAID,EAAEC,GAAGW,KAAK8D,IAAI3E,EAAEE,GAAGF,EAAE4E,gBAAgB,IAAI,OAAO3E,CAAC,CAAjL,GAAqL,GAAGC,EAAEI,MAAMJ,EAAEK,MAAMN,EAAE4E,cAAc3E,EAAEI,MAAM,GAAGJ,EAAEI,MAAMwC,YAAYlC,MAAM,OAAOV,EAAEM,QAAQ,CAACP,GAAGD,EAAEE,EAAE,CAAC,MAAMF,GAAG,CAAC,EAAE,aAAa2B,SAASmD,WAAWvC,WAAWtC,EAAE,GAAG6B,iBAAiB,QAAQ,WAAW,OAAOS,WAAWtC,EAAE,EAAE,GAAG,C",
     "names": [
         "e",
         "t",
         "n",
         "i",
         "r",
         "name",
```

### Comparing `DashAI-0.0.4/DashAI/front/build/static/js/main.4b04b4b2.js.LICENSE.txt` & `DashAI-0.0.9/DashAI/front/build/static/js/main.f87b2cdc.js.LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-/*!
-  Copyright (c) 2018 Jed Watson.
-  Licensed under the MIT License (MIT), see
-  http://jedwatson.github.io/classnames
-*/
-
 /*! regenerator-runtime -- Copyright (c) 2014-present, Facebook, Inc. -- license (MIT): https://github.com/facebook/regenerator/blob/main/LICENSE */
 
 /**
  * @license React
  * react-dom.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
 
 /**
  * @license React
+ * react-is.production.min.js
+ *
+ * Copyright (c) Facebook, Inc. and its affiliates.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
+
+/**
+ * @license React
  * react-jsx-runtime.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
@@ -43,26 +47,53 @@
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
 
 /**
- * @remix-run/router v1.0.1
+ * @mui/styled-engine v5.11.11
+ *
+ * @license MIT
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
+
+/**
+ * @mui/styled-engine v5.13.2
+ *
+ * @license MIT
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
+
+/**
+ * @remix-run/router v1.5.0
+ *
+ * Copyright (c) Remix Software Inc.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE.md file in the root directory of this source tree.
+ *
+ * @license MIT
+ */
+
+/**
+ * React Router DOM v6.10.0
  *
  * Copyright (c) Remix Software Inc.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE.md file in the root directory of this source tree.
  *
  * @license MIT
  */
 
 /**
- * React Router v6.4.1
+ * React Router v6.10.0
  *
  * Copyright (c) Remix Software Inc.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE.md file in the root directory of this source tree.
  *
  * @license MIT
```

### Comparing `DashAI-0.0.4/DashAI/front/build/static/media/Quicksand-Bold.a0a11318dd0b528da77d.ttf` & `DashAI-0.0.9/DashAI/front/build/static/media/Quicksand-Bold.a0a11318dd0b528da77d.ttf`

 * *Files identical despite different names*

