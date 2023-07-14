# Comparing `tmp/lennybot-1.0.8.tar.gz` & `tmp/lennybot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lennybot-1.0.8.tar", last modified: Wed Feb  8 15:59:41 2023, max compression
+gzip compressed data, was "lennybot-1.0.9.tar", last modified: Wed Feb  8 16:02:33 2023, max compression
```

## Comparing `lennybot-1.0.8.tar` & `lennybot-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.038087 lennybot-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 15:58:07.000000 lennybot-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-02-08 15:59:41.038087 lennybot-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-02-08 15:58:07.000000 lennybot-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 15:58:07.000000 lennybot-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 15:59:41.038087 lennybot-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-08 15:58:07.000000 lennybot-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.030088 lennybot-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot/
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/download_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/iaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/remove_checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/update_dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/update_image_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/actions/update_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot/config/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot/helper/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/lennybot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot/model/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/model/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot/service/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.038087 lennybot-1.0.8/src/lennybot/service/source/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/source/isource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/source/source_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-08 15:58:07.000000 lennybot-1.0.8/src/lennybot/service/source/source_github_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:59:41.034088 lennybot-1.0.8/src/lennybot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-02-08 15:59:41.000000 lennybot-1.0.8/src/lennybot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-08 15:59:41.000000 lennybot-1.0.8/src/lennybot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 15:59:41.000000 lennybot-1.0.8/src/lennybot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 15:59:41.000000 lennybot-1.0.8/src/lennybot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-08 15:59:41.000000 lennybot-1.0.8/src/lennybot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-08 15:59:41.000000 lennybot-1.0.8/src/lennybot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-08 15:58:07.000000 lennybot-1.0.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.220410 lennybot-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 16:01:13.000000 lennybot-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-02-08 16:02:33.220410 lennybot-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-02-08 16:01:13.000000 lennybot-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 16:01:13.000000 lennybot-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 16:02:33.220410 lennybot-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-08 16:01:13.000000 lennybot-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.212411 lennybot-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/download_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/iaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/remove_checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/update_dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/update_image_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/actions/update_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/lennybot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/model/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot/service/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/source/isource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/source/source_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-08 16:01:13.000000 lennybot-1.0.9/src/lennybot/service/source/source_github_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 16:02:33.216410 lennybot-1.0.9/src/lennybot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-02-08 16:02:33.000000 lennybot-1.0.9/src/lennybot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-08 16:02:33.000000 lennybot-1.0.9/src/lennybot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 16:02:33.000000 lennybot-1.0.9/src/lennybot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 16:02:33.000000 lennybot-1.0.9/src/lennybot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-08 16:02:33.000000 lennybot-1.0.9/src/lennybot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-08 16:02:33.000000 lennybot-1.0.9/src/lennybot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-08 16:01:13.000000 lennybot-1.0.9/version.txt
```

### Comparing `lennybot-1.0.8/LICENSE` & `lennybot-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/PKG-INFO` & `lennybot-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennybot
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic Updates for Kustomize Resources
 Home-page: http://github.com/raynigon/lennybot
 Author: Simon Schneider
 Author-email: dev@raynigon.com
 Project-URL: Bug Reports, https://github.com/raynigon/lennybot/issues
 Project-URL: Source, https://github.com/raynigon/lennybot/
 Keywords: kustomize
```

### Comparing `lennybot-1.0.8/README.md` & `lennybot-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/setup.py` & `lennybot-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/__init__.py` & `lennybot-1.0.9/src/lennybot/__init__.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/actions/__init__.py` & `lennybot-1.0.9/src/lennybot/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/actions/download_resources.py` & `lennybot-1.0.9/src/lennybot/actions/download_resources.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/actions/remove_checksums.py` & `lennybot-1.0.9/src/lennybot/actions/remove_checksums.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/actions/update_dockerfile.py` & `lennybot-1.0.9/src/lennybot/actions/update_dockerfile.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/actions/update_image_tag.py` & `lennybot-1.0.9/src/lennybot/actions/update_image_tag.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/actions/update_yaml.py` & `lennybot-1.0.9/src/lennybot/actions/update_yaml.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/config/config.py` & `lennybot-1.0.9/src/lennybot/config/config.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/lennybot.py` & `lennybot-1.0.9/src/lennybot/lennybot.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/model/plan.py` & `lennybot-1.0.9/src/lennybot/model/plan.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/model/state.py` & `lennybot-1.0.9/src/lennybot/model/state.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/service/apply.py` & `lennybot-1.0.9/src/lennybot/service/apply.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/service/github.py` & `lennybot-1.0.9/src/lennybot/service/github.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/service/plan.py` & `lennybot-1.0.9/src/lennybot/service/plan.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/service/source/source_github.py` & `lennybot-1.0.9/src/lennybot/service/source/source_github.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot/service/source/source_github_query.py` & `lennybot-1.0.9/src/lennybot/service/source/source_github_query.py`

 * *Files identical despite different names*

### Comparing `lennybot-1.0.8/src/lennybot.egg-info/PKG-INFO` & `lennybot-1.0.9/src/lennybot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennybot
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic Updates for Kustomize Resources
 Home-page: http://github.com/raynigon/lennybot
 Author: Simon Schneider
 Author-email: dev@raynigon.com
 Project-URL: Bug Reports, https://github.com/raynigon/lennybot/issues
 Project-URL: Source, https://github.com/raynigon/lennybot/
 Keywords: kustomize
```

### Comparing `lennybot-1.0.8/src/lennybot.egg-info/SOURCES.txt` & `lennybot-1.0.9/src/lennybot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

