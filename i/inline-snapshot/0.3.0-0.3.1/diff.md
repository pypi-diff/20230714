# Comparing `tmp/inline_snapshot-0.3.0.tar.gz` & `tmp/inline_snapshot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.3.0.tar", max compression
+gzip compressed data, was "inline_snapshot-0.3.1.tar", max compression
```

## Comparing `inline_snapshot-0.3.0.tar` & `inline_snapshot-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.3.0/LICENSE
--rw-r--r--   0        0        0     3075 2023-07-09 19:32:08.031840 inline_snapshot-0.3.0/README.md
--rw-r--r--   0        0        0       62 2023-07-12 16:51:48.846767 inline_snapshot-0.3.0/inline_snapshot/__init__.py
--rw-r--r--   0        0        0      248 2023-07-09 13:33:21.148429 inline_snapshot-0.3.0/inline_snapshot/_format.py
--rw-r--r--   0        0        0    14832 2023-07-12 16:34:33.544136 inline_snapshot-0.3.0/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0     5448 2023-07-09 13:33:21.148429 inline_snapshot-0.3.0/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0     5445 2023-07-09 14:55:53.631461 inline_snapshot-0.3.0/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     1620 2023-07-12 16:51:48.846767 inline_snapshot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 inline_snapshot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3075 2023-07-13 22:23:21.207977 inline_snapshot-0.3.1/README.md
+-rw-r--r--   0        0        0       86 2023-07-14 07:14:59.218737 inline_snapshot-0.3.1/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-12 20:13:28.911699 inline_snapshot-0.3.1/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    14999 2023-07-14 07:01:48.261328 inline_snapshot-0.3.1/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0     5448 2023-07-13 18:14:22.460873 inline_snapshot-0.3.1/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0     5445 2023-07-09 14:55:53.631461 inline_snapshot-0.3.1/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     1620 2023-07-14 07:14:59.218737 inline_snapshot-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 inline_snapshot-0.3.1/PKG-INFO
```

### Comparing `inline_snapshot-0.3.0/LICENSE` & `inline_snapshot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.3.0/README.md` & `inline_snapshot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.3.0/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.3.1/inline_snapshot/_inline_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,22 +528,27 @@
         tokens = list(self._expr.source.asttokens().get_tokens(self._expr.node))
         assert tokens[0].string == "snapshot"
         assert tokens[1].string == "("
         assert tokens[-1].string == ")"
 
         change.set_tags("inline_snapshot")
 
+        needs_fix = self._value._needs_fix()
+        needs_create = self._value._needs_create()
+        needs_trim = self._value._needs_trim()
+
         if (
             _update_flags.update
+            and not (needs_fix or needs_create or needs_trim)
             or _update_flags.fix
-            and self._value._needs_fix
+            and needs_fix
             or _update_flags.create
-            and self._value._needs_create
+            and needs_create
             or _update_flags.trim
-            and self._value._needs_trim
+            and needs_trim
         ):
             new_value = self._value.get_result(_update_flags)
 
             text = self._format(
                 tokenize.untokenize(self._value_to_token(new_value))
             ).strip()
```

### Comparing `inline_snapshot-0.3.0/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.3.1/inline_snapshot/_rewrite_code.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.3.0/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.3.1/inline_snapshot/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.3.0/pyproject.toml` & `inline_snapshot-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Framework :: Pytest"
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.3.0"
+version = "0.3.1"
 
 [tool.poetry.dependencies]
 asttokens = "^2.0.5"
 black = "^23.3.0"
 click = "^8.1.4"
 executing = "^1.2.0"
 python = "^3.7"
```

### Comparing `inline_snapshot-0.3.0/PKG-INFO` & `inline_snapshot-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.3.0
+Version: 0.3.1
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

