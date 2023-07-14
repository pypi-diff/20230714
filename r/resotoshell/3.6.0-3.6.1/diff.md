# Comparing `tmp/resotoshell-3.6.0.tar.gz` & `tmp/resotoshell-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.6.0.tar", last modified: Fri Jun 30 19:29:51 2023, max compression
+gzip compressed data, was "resotoshell-3.6.1.tar", last modified: Fri Jul 14 17:04:51 2023, max compression
```

## Comparing `resotoshell-3.6.0.tar` & `resotoshell-3.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:48.000000 resotoshell-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 19:29:51.858892 resotoshell-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-30 19:24:48.000000 resotoshell-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-30 19:24:48.000000 resotoshell-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37345 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-30 19:24:48.000000 resotoshell-3.6.0/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:19.000000 resotoshell-3.6.0/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 19:29:51.000000 resotoshell-3.6.0/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 19:29:51.858892 resotoshell-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:51.858892 resotoshell-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 19:24:48.000000 resotoshell-3.6.0/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-06-30 19:24:48.000000 resotoshell-3.6.0/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-30 19:24:48.000000 resotoshell-3.6.0/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:51.858562 resotoshell-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:59:09.000000 resotoshell-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-14 17:04:51.858562 resotoshell-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-14 16:59:09.000000 resotoshell-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-14 16:59:09.000000 resotoshell-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:51.854562 resotoshell-3.6.1/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-14 16:59:09.000000 resotoshell-3.6.1/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-07-14 16:59:09.000000 resotoshell-3.6.1/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-14 16:59:09.000000 resotoshell-3.6.1/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37474 2023-07-14 16:59:09.000000 resotoshell-3.6.1/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-14 16:59:09.000000 resotoshell-3.6.1/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-07-14 16:59:09.000000 resotoshell-3.6.1/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:51.858562 resotoshell-3.6.1/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-14 17:04:51.000000 resotoshell-3.6.1/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 17:04:51.000000 resotoshell-3.6.1/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:04:51.000000 resotoshell-3.6.1/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 17:04:51.000000 resotoshell-3.6.1/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:49.000000 resotoshell-3.6.1/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-14 17:04:51.000000 resotoshell-3.6.1/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 17:04:51.000000 resotoshell-3.6.1/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 17:04:51.858562 resotoshell-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:51.858562 resotoshell-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 16:59:09.000000 resotoshell-3.6.1/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-07-14 16:59:09.000000 resotoshell-3.6.1/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-14 16:59:09.000000 resotoshell-3.6.1/test/test_protected_files.py
```

### Comparing `resotoshell-3.6.0/PKG-INFO` & `resotoshell-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.6.0
+Version: 3.6.1
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.6.0/README.md` & `resotoshell-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/pyproject.toml` & `resotoshell-3.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotoshell"
-version = "3.6.0"
+version = "3.6.1"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Resoto."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["cloud security"]
 
 dependencies = [
-    "resotolib==3.6.0",
+    "resotolib==3.6.1",
     "prompt-toolkit",
     "rich",
     "resotoclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `resotoshell-3.6.0/resotoshell/__main__.py` & `resotoshell-3.6.1/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/resotoshell/authorized_client.py` & `resotoshell-3.6.1/resotoshell/authorized_client.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/resotoshell/promptsession.py` & `resotoshell-3.6.1/resotoshell/promptsession.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 from prompt_toolkit.document import Document
 from prompt_toolkit.history import FileHistory, History
 from prompt_toolkit.styles import Style
 from resotoclient.async_client import ResotoClient
 from resotoclient.models import Property
 
-from resotolib.json import from_json, register_json
+from resotolib.json import from_json, register_json, value_in_path
 from resotolib.logger import log
 from resotolib.types import JsonElement
 
 
 def cut_document_remaining(document: Document, span: Tuple[int, int]) -> Document:
     remaining = document.text_before_cursor[span[0] : span[1]]
     return Document(
@@ -803,29 +803,29 @@
                 result.append(name)
 
             kd = model.kinds.get(kind)
             if kd is not None and kd.properties:
                 result.extend(name + "." + pp for prop in kd.properties for pp in path(prop))
             return result
 
-        aggregate_roots = {
-            k: v for k, v in model.kinds.items() if getattr(v, "aggregate_root", True) and v.properties is not None
-        }
+        aggregate_roots = {k: v for k, v in model.kinds.items() if v.aggregate_root and v.properties is not None}
+        # filter out all dynamically created kinds
+        visible_kinds = sorted(k for k, v in aggregate_roots.items() if value_in_path(v.metadata, ["dynamic"]) is None)
 
         known_props = {p for v in aggregate_roots.values() for prop in v.properties or [] for p in path(prop)}
         info = await client.cli_info()
         cmds = [
             from_json(cmd, CommandInfo)
             for cmd in (info.get("commands", []) + info.get("alias_templates", []) + info.get("infra_app_aliases", []))
         ]
         lookup = {cmd.name: cmd for cmd in cmds}
         for alias, cmd in info.get("alias_names", {}).items():
             if cmd in lookup and alias not in lookup:
                 cmds.append(evolve(lookup[cmd], name=alias, is_alias=True))
-        return cmds, sorted(aggregate_roots.keys()), sorted(known_props)
+        return cmds, visible_kinds, sorted(known_props)
     except Exception as ex:
         log.warning(
             f"Can not load metadata from core: {ex}. No suggestions as fallback.",
             exc_info=ex,
         )
         return [], [], []
```

### Comparing `resotoshell-3.6.0/resotoshell/protected_files.py` & `resotoshell-3.6.1/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/resotoshell/shell.py` & `resotoshell-3.6.1/resotoshell/shell.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.6.1/resotoshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.6.0
+Version: 3.6.1
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.6.0/resotoshell.egg-info/SOURCES.txt` & `resotoshell-3.6.1/resotoshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/test/test_promptsession.py` & `resotoshell-3.6.1/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.6.0/test/test_protected_files.py` & `resotoshell-3.6.1/test/test_protected_files.py`

 * *Files identical despite different names*

