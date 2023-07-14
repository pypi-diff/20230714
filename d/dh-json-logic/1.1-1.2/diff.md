# Comparing `tmp/dh_json_logic-1.1.tar.gz` & `tmp/dh_json_logic-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh_json_logic-1.1.tar", max compression
+gzip compressed data, was "dh_json_logic-1.2.tar", max compression
```

## Comparing `dh_json_logic-1.1.tar` & `dh_json_logic-1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-14 12:23:34.017503 dh_json_logic-1.1/LICENSE
--rw-r--r--   0        0        0     3168 2023-07-14 12:23:34.017503 dh_json_logic-1.1/README.md
--rw-r--r--   0        0        0    31272 2023-07-14 12:23:34.017503 dh_json_logic-1.1/dh_json_logic/__init__.py
--rw-r--r--   0        0        0     1156 2023-07-14 12:23:34.017503 dh_json_logic-1.1/pyproject.toml
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 dh_json_logic-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-14 12:48:30.491825 dh_json_logic-1.2/LICENSE
+-rw-r--r--   0        0        0     3168 2023-07-14 12:48:30.491825 dh_json_logic-1.2/README.md
+-rw-r--r--   0        0        0    31272 2023-07-14 12:48:30.491825 dh_json_logic-1.2/dh_json_logic/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-14 12:48:30.491825 dh_json_logic-1.2/pyproject.toml
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 dh_json_logic-1.2/PKG-INFO
```

### Comparing `dh_json_logic-1.1/LICENSE` & `dh_json_logic-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.1/README.md` & `dh_json_logic-1.2/README.md`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.1/dh_json_logic/__init__.py` & `dh_json_logic-1.2/dh_json_logic/__init__.py`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.1/pyproject.toml` & `dh_json_logic-1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 [build-system]
 requires = [ "poetry_core>=1.6.1" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dh-json-logic"
-version = "1.1"
+version = "1.2"
 description = "A fork of https://github.com/YaraslauZhylko/json-logic-py/"
 readme="README.md"
 authors = [ "dearhealth" ]
+homepage = "https://github.com/dearhealth/json-logic-py"
+repository = "https://github.com/dearhealth/json-logic-py"
 
   [tool.poetry.dependencies]
     python = "^3.10"
 
 
   [tool.poetry.dev-dependencies]
   pytest = "^7.4.0"
```

### Comparing `dh_json_logic-1.1/PKG-INFO` & `dh_json_logic-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dh-json-logic
-Version: 1.1
+Version: 1.2
 Summary: A fork of https://github.com/YaraslauZhylko/json-logic-py/
+Home-page: https://github.com/dearhealth/json-logic-py
 Author: dearhealth
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/dearhealth/json-logic-py
 Description-Content-Type: text/markdown
 
 # json-logic-py
 **NOTE:** This is fork of https://github.com/YaraslauZhylko/json-logic-py/ created for use in our internal projects.
 
 
 ## Introduction
```

