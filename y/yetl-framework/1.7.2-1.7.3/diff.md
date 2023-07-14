# Comparing `tmp/yetl-framework-1.7.2.tar.gz` & `tmp/yetl-framework-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.7.2.tar", last modified: Thu Jul 13 19:06:18 2023, max compression
+gzip compressed data, was "yetl-framework-1.7.3.tar", last modified: Fri Jul 14 10:14:36 2023, max compression
```

## Comparing `yetl-framework-1.7.2.tar` & `yetl-framework-1.7.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.782158 yetl-framework-1.7.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-13 19:06:18.782158 yetl-framework-1.7.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-13 19:06:18.782158 yetl-framework-1.7.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1461 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.774158 yetl-framework-1.7.2/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.774158 yetl-framework-1.7.2/yetl/_resources/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/_resources/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/_resources/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/_resources/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/_resources/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/_resources/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/_resources/sibytes_yetl_tables_schema.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.778158 yetl-framework-1.7.2/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3398 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.778158 yetl-framework-1.7.2/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16878 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.778158 yetl-framework-1.7.2/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.778158 yetl-framework-1.7.2/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4980 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.778158 yetl-framework-1.7.2/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1555 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.778158 yetl-framework-1.7.2/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-13 19:05:22.000000 yetl-framework-1.7.2/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 19:06:18.782158 yetl-framework-1.7.2/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-13 19:06:18.000000 yetl-framework-1.7.2/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1361 2023-07-13 19:06:18.000000 yetl-framework-1.7.2/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-13 19:06:18.000000 yetl-framework-1.7.2/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-13 19:06:18.000000 yetl-framework-1.7.2/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-07-13 19:06:18.000000 yetl-framework-1.7.2/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-13 19:06:18.000000 yetl-framework-1.7.2/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.115992 yetl-framework-1.7.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-14 10:14:36.115992 yetl-framework-1.7.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1461 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/_resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_tables_schema.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3398 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16878 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4980 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1555 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1361 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.7.2/PKG-INFO` & `yetl-framework-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.7.2
+Version: 1.7.3
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.7.2/README.md` & `yetl-framework-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/setup.py` & `yetl-framework-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.7.2",
+    version="1.7.3",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.7.2/yetl/__main__.py` & `yetl-framework-1.7.3/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/_resources/sibytes_yetl_pipeline_schema.json` & `yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/_resources/sibytes_yetl_project_schema.json` & `yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/_resources/sibytes_yetl_tables_schema.json` & `yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_tables_schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444445%*

 * *Differences: {"'required'": '{delete: [2, 1]}'}*

```diff
@@ -355,13 +355,11 @@
         "version": {
             "description": "version of yetl that the configuration is compatible with",
             "pattern": "^(\\d+\\.)?(\\d+\\.)?(\\*|\\d+)$",
             "type": "string"
         }
     },
     "required": [
-        "version",
-        "landing",
-        "raw"
+        "version"
     ],
     "type": "object"
 }
```

### Comparing `yetl-framework-1.7.2/yetl/cli/_init.py` & `yetl-framework-1.7.3/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.7.3/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/__init__.py` & `yetl-framework-1.7.3/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_config.py` & `yetl-framework-1.7.3/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_decorators.py` & `yetl-framework-1.7.3/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_logging_config.py` & `yetl-framework-1.7.3/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_project.py` & `yetl-framework-1.7.3/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_spark_context.py` & `yetl-framework-1.7.3/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_tables.py` & `yetl-framework-1.7.3/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_timeslice.py` & `yetl-framework-1.7.3/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/_utils.py` & `yetl-framework-1.7.3/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/deltalake.py` & `yetl-framework-1.7.3/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/table/_deltalake.py` & `yetl-framework-1.7.3/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/table/_factory.py` & `yetl-framework-1.7.3/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/table/_read.py` & `yetl-framework-1.7.3/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/config/table/_table.py` & `yetl-framework-1.7.3/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/validation/_validate.py` & `yetl-framework-1.7.3/yetl/validation/_validate.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/workflow/_dlt.py` & `yetl-framework-1.7.3/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.7.3/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.2/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.7.3/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.7.2
+Version: 1.7.3
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.7.2/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.7.3/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

