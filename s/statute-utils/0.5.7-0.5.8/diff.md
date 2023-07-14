# Comparing `tmp/statute_utils-0.5.7.tar.gz` & `tmp/statute_utils-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.7.tar", max compression
+gzip compressed data, was "statute_utils-0.5.8.tar", max compression
```

## Comparing `statute_utils-0.5.7.tar` & `statute_utils-0.5.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.7/LICENSE
--rw-r--r--   0        0        0     3593 2023-07-14 16:18:39.431381 statute_utils-0.5.7/README.md
--rw-r--r--   0        0        0     1314 2023-07-14 17:02:40.274795 statute_utils-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      678 2023-07-14 16:17:42.904400 statute_utils-0.5.7/statute_utils/__init__.py
--rw-r--r--   0        0        0      460 2023-07-14 10:30:59.403468 statute_utils-0.5.7/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-14 14:09:59.832215 statute_utils-0.5.7/statute_utils/components/builder.py
--rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.5.7/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.7/statute_utils/components/short.py
--rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.7/statute_utils/components/utils.py
--rw-r--r--   0        0        0     3963 2023-07-14 16:17:14.380273 statute_utils-0.5.7/statute_utils/display.py
--rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.7/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.7/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.7/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.7/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.7/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.7/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.7/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.7/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.7/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0       87 2023-07-14 12:22:55.153217 statute_utils-0.5.7/statute_utils/templates/branch.html
--rw-r--r--   0        0        0     1114 2023-07-14 18:24:17.829710 statute_utils-0.5.7/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     2224 2023-07-14 18:27:08.881995 statute_utils-0.5.7/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     6519 2023-07-14 12:30:11.704539 statute_utils-0.5.7/statute_utils/tree.py
--rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 statute_utils-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.8/LICENSE
+-rw-r--r--   0        0        0     3593 2023-07-14 16:18:39.431381 statute_utils-0.5.8/README.md
+-rw-r--r--   0        0        0     1314 2023-07-14 18:28:45.360571 statute_utils-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      678 2023-07-14 16:17:42.904400 statute_utils-0.5.8/statute_utils/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-14 10:30:59.403468 statute_utils-0.5.8/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-14 14:09:59.832215 statute_utils-0.5.8/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.5.8/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.8/statute_utils/components/short.py
+-rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.8/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     3963 2023-07-14 16:17:14.380273 statute_utils-0.5.8/statute_utils/display.py
+-rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.8/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.8/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.8/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.8/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.8/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.8/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.8/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.8/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.8/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0       87 2023-07-14 12:22:55.153217 statute_utils-0.5.8/statute_utils/templates/branch.html
+-rw-r--r--   0        0        0     1114 2023-07-14 18:24:17.829710 statute_utils-0.5.8/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     2224 2023-07-14 18:27:08.881995 statute_utils-0.5.8/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     6519 2023-07-14 12:30:11.704539 statute_utils-0.5.8/statute_utils/tree.py
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 statute_utils-0.5.8/PKG-INFO
```

### Comparing `statute_utils-0.5.7/LICENSE` & `statute_utils-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/README.md` & `statute_utils-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/pyproject.toml` & `statute_utils-0.5.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.7"
+version = "0.5.8"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.5.7/statute_utils/__init__.py` & `statute_utils-0.5.8/statute_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/components/builder.py` & `statute_utils-0.5.8/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/components/category.py` & `statute_utils-0.5.8/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/components/short.py` & `statute_utils-0.5.8/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/components/utils.py` & `statute_utils-0.5.8/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/display.py` & `statute_utils-0.5.8/statute_utils/display.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/main.py` & `statute_utils-0.5.8/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/models.py` & `statute_utils-0.5.8/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/models_names.py` & `statute_utils-0.5.8/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/models_serials.py` & `statute_utils-0.5.8/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/recipes/digits.py` & `statute_utils-0.5.8/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/recipes/spain.py` & `statute_utils-0.5.8/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/templates/tree.css` & `statute_utils-0.5.8/statute_utils/templates/tree.css`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/templates/tree.html` & `statute_utils-0.5.8/statute_utils/templates/tree.html`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/statute_utils/tree.py` & `statute_utils-0.5.8/statute_utils/tree.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.7/PKG-INFO` & `statute_utils-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.5.7
+Version: 0.5.8
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

