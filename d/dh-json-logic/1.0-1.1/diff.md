# Comparing `tmp/dh_json_logic-1.0.tar.gz` & `tmp/dh_json_logic-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh_json_logic-1.0.tar", max compression
+gzip compressed data, was "dh_json_logic-1.1.tar", max compression
```

## Comparing `dh_json_logic-1.0.tar` & `dh_json_logic-1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-14 11:54:55.540565 dh_json_logic-1.0/LICENSE
--rw-r--r--   0        0        0    31272 2023-07-14 11:54:55.540565 dh_json_logic-1.0/dh_json_logic/__init__.py
--rw-r--r--   0        0        0     1079 2023-07-14 11:54:55.540565 dh_json_logic-1.0/pyproject.toml
--rw-r--r--   0        0        0      263 1970-01-01 00:00:00.000000 dh_json_logic-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-14 12:23:34.017503 dh_json_logic-1.1/LICENSE
+-rw-r--r--   0        0        0     3168 2023-07-14 12:23:34.017503 dh_json_logic-1.1/README.md
+-rw-r--r--   0        0        0    31272 2023-07-14 12:23:34.017503 dh_json_logic-1.1/dh_json_logic/__init__.py
+-rw-r--r--   0        0        0     1156 2023-07-14 12:23:34.017503 dh_json_logic-1.1/pyproject.toml
+-rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 dh_json_logic-1.1/PKG-INFO
```

### Comparing `dh_json_logic-1.0/LICENSE` & `dh_json_logic-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.0/dh_json_logic/__init__.py` & `dh_json_logic-1.1/dh_json_logic/__init__.py`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.0/pyproject.toml` & `dh_json_logic-1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 [build-system]
 requires = [ "poetry_core>=1.6.1" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dh-json-logic"
-version = "1.0"
-description = ""
+version = "1.1"
+description = "A fork of https://github.com/YaraslauZhylko/json-logic-py/"
+readme="README.md"
 authors = [ "dearhealth" ]
 
   [tool.poetry.dependencies]
     python = "^3.10"
 
 
   [tool.poetry.dev-dependencies]
```

