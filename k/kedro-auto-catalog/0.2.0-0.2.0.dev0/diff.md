# Comparing `tmp/kedro_auto_catalog-0.2.0.tar.gz` & `tmp/kedro_auto_catalog-0.2.0.dev0.tar.gz`

## Comparing `kedro_auto_catalog-0.2.0.tar` & `kedro_auto_catalog-0.2.0.dev0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/.kedro-auto-catalog-copier-answers.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/kedro_auto_catalog/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/kedro_auto_catalog/__init__.py
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/kedro_auto_catalog/cli.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/tests/test_dummy.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/README.md
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/.kedro-auto-catalog-copier-answers.yml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/kedro_auto_catalog/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/kedro_auto_catalog/__init__.py
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/kedro_auto_catalog/cli.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/tests/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/tests/test_dummy.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 kedro_auto_catalog-0.2.0.dev0/PKG-INFO
```

### Comparing `kedro_auto_catalog-0.2.0/kedro_auto_catalog/cli.py` & `kedro_auto_catalog-0.2.0.dev0/kedro_auto_catalog/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_auto_catalog-0.2.0/.gitignore` & `kedro_auto_catalog-0.2.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_auto_catalog-0.2.0/LICENSE.txt` & `kedro_auto_catalog-0.2.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro_auto_catalog-0.2.0/README.md` & `kedro_auto_catalog-0.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `kedro_auto_catalog-0.2.0/pyproject.toml` & `kedro_auto_catalog-0.2.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro_auto_catalog-0.2.0/PKG-INFO` & `kedro_auto_catalog-0.2.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-auto-catalog
-Version: 0.2.0
+Version: 0.2.0.dev0
 Summary: A configurable replacement for `kedro catalog create`.
 Project-URL: Documentation, https://github.com/waylonwalker/kedro-auto-catalog#readme
 Project-URL: Issues, https://github.com/waylonwalker/kedro-auto-catalog/issues
 Project-URL: Source, https://github.com/waylonwalker/kedro-auto-catalog
 Project-URL: Changelog, https://github.com/waylonwalker/kedro-auto-catalog
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
```

