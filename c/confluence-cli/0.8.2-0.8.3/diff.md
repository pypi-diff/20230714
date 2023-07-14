# Comparing `tmp/confluence_cli-0.8.2.tar.gz` & `tmp/confluence_cli-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluence_cli-0.8.2.tar", max compression
+gzip compressed data, was "confluence_cli-0.8.3.tar", max compression
```

## Comparing `confluence_cli-0.8.2.tar` & `confluence_cli-0.8.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2022-12-03 16:21:12.562517 confluence_cli-0.8.2/LICENSE.txt
--rw-r--r--   0        0        0      939 2022-12-12 18:03:51.829619 confluence_cli-0.8.2/README.md
--rw-r--r--   0        0        0      233 2022-12-03 16:21:12.318517 confluence_cli-0.8.2/confluence_cli/cli/__init__.py
--rw-r--r--   0        0        0     1860 2022-12-03 16:21:12.310517 confluence_cli-0.8.2/confluence_cli/cli/comala_api.py
--rw-r--r--   0        0        0     7219 2023-01-30 19:37:24.723228 confluence_cli-0.8.2/confluence_cli/cli/confluence_async.py
--rw-r--r--   0        0        0     1230 2022-12-12 17:53:44.181742 confluence_cli-0.8.2/confluence_cli/cli/confluence_limited.py
--rw-r--r--   0        0        0    13393 2022-12-12 21:17:59.128698 confluence_cli-0.8.2/confluence_cli/cli/confluence_wrapper.py
--rw-r--r--   0        0        0     8059 2023-01-30 14:53:18.184682 confluence_cli-0.8.2/confluence_cli/cli/paginators.py
--rw-r--r--   0        0        0     3509 2023-01-30 13:48:54.049440 confluence_cli-0.8.2/confluence_cli/cli/types.py
--rw-r--r--   0        0        0     2577 2023-07-08 20:52:47.543022 confluence_cli-0.8.2/confluence_cli/cli/utils.py
--rw-r--r--   0        0        0      815 2023-07-11 14:35:29.142344 confluence_cli-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 confluence_cli-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 16:21:12.562517 confluence_cli-0.8.3/LICENSE.txt
+-rw-r--r--   0        0        0      939 2022-12-12 18:03:51.829619 confluence_cli-0.8.3/README.md
+-rw-r--r--   0        0        0      233 2022-12-03 16:21:12.318517 confluence_cli-0.8.3/confluence_cli/cli/__init__.py
+-rw-r--r--   0        0        0     1860 2022-12-03 16:21:12.310517 confluence_cli-0.8.3/confluence_cli/cli/comala_api.py
+-rw-r--r--   0        0        0     7219 2023-01-30 19:37:24.723228 confluence_cli-0.8.3/confluence_cli/cli/confluence_async.py
+-rw-r--r--   0        0        0     1230 2022-12-12 17:53:44.181742 confluence_cli-0.8.3/confluence_cli/cli/confluence_limited.py
+-rw-r--r--   0        0        0    13393 2022-12-12 21:17:59.128698 confluence_cli-0.8.3/confluence_cli/cli/confluence_wrapper.py
+-rw-r--r--   0        0        0     8059 2023-01-30 14:53:18.184682 confluence_cli-0.8.3/confluence_cli/cli/paginators.py
+-rw-r--r--   0        0        0     3509 2023-01-30 13:48:54.049440 confluence_cli-0.8.3/confluence_cli/cli/types.py
+-rw-r--r--   0        0        0     2622 2023-07-14 12:50:14.252042 confluence_cli-0.8.3/confluence_cli/cli/utils.py
+-rw-r--r--   0        0        0      815 2023-07-14 12:50:25.951292 confluence_cli-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 confluence_cli-0.8.3/PKG-INFO
```

### Comparing `confluence_cli-0.8.2/LICENSE.txt` & `confluence_cli-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/README.md` & `confluence_cli-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/comala_api.py` & `confluence_cli-0.8.3/confluence_cli/cli/comala_api.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/confluence_async.py` & `confluence_cli-0.8.3/confluence_cli/cli/confluence_async.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/confluence_limited.py` & `confluence_cli-0.8.3/confluence_cli/cli/confluence_limited.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/confluence_wrapper.py` & `confluence_cli-0.8.3/confluence_cli/cli/confluence_wrapper.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/paginators.py` & `confluence_cli-0.8.3/confluence_cli/cli/paginators.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/types.py` & `confluence_cli-0.8.3/confluence_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `confluence_cli-0.8.2/confluence_cli/cli/utils.py` & `confluence_cli-0.8.3/confluence_cli/cli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 def type_wrap(content):
     """ Wrap content in a type
 
     :param content:   The content to wrap    
     :return:          The wrapped content    
     """
+    if content is None:
+        return None
+
     types = {
         "page": Page,
         "global": Space,
         "blogpost": BlogPost,
         "attachment": Attachment,
         "comment": Comment,
         "workflowName": NavigableDict,
```

### Comparing `confluence_cli-0.8.2/pyproject.toml` & `confluence_cli-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "confluence-cli"
-version = "0.8.2"
+version = "0.8.3"
 description = "Just another Atlassian Confluence API cli extension"
 authors = ["J. Andres Guerrero <juguerre@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "confluence_cli/cli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `confluence_cli-0.8.2/PKG-INFO` & `confluence_cli-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluence-cli
-Version: 0.8.2
+Version: 0.8.3
 Summary: Just another Atlassian Confluence API cli extension
 License: MIT
 Author: J. Andres Guerrero
 Author-email: juguerre@gmail.com
 Requires-Python: >=3.8.0,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

