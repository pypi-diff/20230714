# Comparing `tmp/micrograd-utils-0.0.2.tar.gz` & `tmp/micrograd-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrograd-utils-0.0.2.tar", last modified: Fri Jul 14 19:14:07 2023, max compression
+gzip compressed data, was "micrograd-utils-0.0.3.tar", last modified: Fri Jul 14 19:29:42 2023, max compression
```

## Comparing `micrograd-utils-0.0.2.tar` & `micrograd-utils-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:14:07.799799 micrograd-utils-0.0.2/
--rw-r--r--   0 valerio   (1000) valerio   (1000)     1073 2023-07-14 18:58:40.000000 micrograd-utils-0.0.2/LICENSE
--rw-r--r--   0 valerio   (1000) valerio   (1000)      610 2023-07-14 19:14:07.799799 micrograd-utils-0.0.2/PKG-INFO
--rw-r--r--   0 valerio   (1000) valerio   (1000)      171 2023-07-14 19:02:47.000000 micrograd-utils-0.0.2/README.md
--rw-r--r--   0 valerio   (1000) valerio   (1000)      554 2023-07-14 19:14:02.000000 micrograd-utils-0.0.2/pyproject.toml
--rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2023-07-14 19:14:07.799799 micrograd-utils-0.0.2/setup.cfg
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:14:07.795799 micrograd-utils-0.0.2/src/
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:14:07.797799 micrograd-utils-0.0.2/src/micrograd_utils/
--rw-r--r--   0 valerio   (1000) valerio   (1000)        0 2023-07-14 18:58:40.000000 micrograd-utils-0.0.2/src/micrograd_utils/__init__.py
--rwxr-xr-x   0 valerio   (1000) valerio   (1000)      689 2023-07-14 18:59:48.000000 micrograd-utils-0.0.2/src/micrograd_utils/utils.py
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:14:07.798799 micrograd-utils-0.0.2/src/micrograd_utils.egg-info/
--rw-r--r--   0 valerio   (1000) valerio   (1000)      610 2023-07-14 19:14:07.000000 micrograd-utils-0.0.2/src/micrograd_utils.egg-info/PKG-INFO
--rw-r--r--   0 valerio   (1000) valerio   (1000)      311 2023-07-14 19:14:07.000000 micrograd-utils-0.0.2/src/micrograd_utils.egg-info/SOURCES.txt
--rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2023-07-14 19:14:07.000000 micrograd-utils-0.0.2/src/micrograd_utils.egg-info/dependency_links.txt
--rw-r--r--   0 valerio   (1000) valerio   (1000)       44 2023-07-14 19:14:07.000000 micrograd-utils-0.0.2/src/micrograd_utils.egg-info/entry_points.txt
--rw-r--r--   0 valerio   (1000) valerio   (1000)       16 2023-07-14 19:14:07.000000 micrograd-utils-0.0.2/src/micrograd_utils.egg-info/top_level.txt
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:29:42.718918 micrograd-utils-0.0.3/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     1073 2023-07-14 18:58:40.000000 micrograd-utils-0.0.3/LICENSE
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      624 2023-07-14 19:29:42.717918 micrograd-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      173 2023-07-14 19:19:19.000000 micrograd-utils-0.0.3/README.md
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      519 2023-07-14 19:29:38.000000 micrograd-utils-0.0.3/pyproject.toml
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2023-07-14 19:29:42.719918 micrograd-utils-0.0.3/setup.cfg
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:29:42.712918 micrograd-utils-0.0.3/src/
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:29:42.715918 micrograd-utils-0.0.3/src/micrograd_utils/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        0 2023-07-14 18:58:40.000000 micrograd-utils-0.0.3/src/micrograd_utils/__init__.py
+-rwxr-xr-x   0 valerio   (1000) valerio   (1000)      689 2023-07-14 18:59:48.000000 micrograd-utils-0.0.3/src/micrograd_utils/utils.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-07-14 19:29:42.717918 micrograd-utils-0.0.3/src/micrograd_utils.egg-info/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      624 2023-07-14 19:29:42.000000 micrograd-utils-0.0.3/src/micrograd_utils.egg-info/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      265 2023-07-14 19:29:42.000000 micrograd-utils-0.0.3/src/micrograd_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2023-07-14 19:29:42.000000 micrograd-utils-0.0.3/src/micrograd_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       16 2023-07-14 19:29:42.000000 micrograd-utils-0.0.3/src/micrograd_utils.egg-info/top_level.txt
```

### Comparing `micrograd-utils-0.0.2/LICENSE` & `micrograd-utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `micrograd-utils-0.0.2/PKG-INFO` & `micrograd-utils-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micrograd-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: utils for micrograd
 Author-email: Valerio Iacobucci <valerio@valerioiacobucci.com>
-Project-URL: Homepage, https://github.com/iacobucci/vml
+Project-URL: Homepage, https://github.com/iacobucci/micrograd-utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # micrograd-utils
-These are some scrap utils i am experimenting on while learning about machine learning, together with [micrograd](https://github.com/karpathy/micrograd)
+These are some scrap *utils* i am randomly using while experimenting on machine learning, together with [micrograd](https://github.com/karpathy/micrograd)
```

### Comparing `micrograd-utils-0.0.2/src/micrograd_utils/utils.py` & `micrograd-utils-0.0.3/src/micrograd_utils/utils.py`

 * *Files identical despite different names*

### Comparing `micrograd-utils-0.0.2/src/micrograd_utils.egg-info/PKG-INFO` & `micrograd-utils-0.0.3/src/micrograd_utils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micrograd-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: utils for micrograd
 Author-email: Valerio Iacobucci <valerio@valerioiacobucci.com>
-Project-URL: Homepage, https://github.com/iacobucci/vml
+Project-URL: Homepage, https://github.com/iacobucci/micrograd-utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # micrograd-utils
-These are some scrap utils i am experimenting on while learning about machine learning, together with [micrograd](https://github.com/karpathy/micrograd)
+These are some scrap *utils* i am randomly using while experimenting on machine learning, together with [micrograd](https://github.com/karpathy/micrograd)
```

