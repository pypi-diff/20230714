# Comparing `tmp/idealforms-0.0.2.tar.gz` & `tmp/idealforms-0.0.9.tar.gz`

## Comparing `idealforms-0.0.2.tar` & `idealforms-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 idealforms-0.0.2/.env.example
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 idealforms-0.0.2/requirements.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 idealforms-0.0.2/requirements_dev.txt
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 idealforms-0.0.2/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idealforms-0.0.2/src/idealforms/__init__.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 idealforms-0.0.2/src/idealforms/bar.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 idealforms-0.0.2/src/idealforms/formatters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idealforms-0.0.2/src/idealforms/py.typed
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 idealforms-0.0.2/tests/bar_test.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 idealforms-0.0.2/tests/formatters_test.py
--rw-r--r--   0        0        0    24281 2020-02-02 00:00:00.000000 idealforms-0.0.2/tests/bar_test_comparison_images/test_bar_out_labels.png
--rw-r--r--   0        0        0    26760 2020-02-02 00:00:00.000000 idealforms-0.0.2/tests/bar_test_comparison_images/test_bar_sort_alpha.png
--rw-r--r--   0        0        0    24395 2020-02-02 00:00:00.000000 idealforms-0.0.2/tests/bar_test_comparison_images/test_bar_sort_values.png
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 idealforms-0.0.2/.gitignore
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 idealforms-0.0.2/LICENSE
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 idealforms-0.0.2/README.md
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 idealforms-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 idealforms-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 idealforms-0.0.9/.env.example
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 idealforms-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 idealforms-0.0.9/requirements_dev.txt
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 idealforms-0.0.9/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idealforms-0.0.9/src/idealforms/__init__.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 idealforms-0.0.9/src/idealforms/bar.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 idealforms-0.0.9/src/idealforms/formatters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 idealforms-0.0.9/src/idealforms/py.typed
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 idealforms-0.0.9/tests/bar_test.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 idealforms-0.0.9/tests/formatters_test.py
+-rw-r--r--   0        0        0    24281 2020-02-02 00:00:00.000000 idealforms-0.0.9/tests/bar_test_comparison_images/test_bar_out_labels.png
+-rw-r--r--   0        0        0    26760 2020-02-02 00:00:00.000000 idealforms-0.0.9/tests/bar_test_comparison_images/test_bar_sort_alpha.png
+-rw-r--r--   0        0        0    24395 2020-02-02 00:00:00.000000 idealforms-0.0.9/tests/bar_test_comparison_images/test_bar_sort_values.png
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 idealforms-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 idealforms-0.0.9/LICENSE
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 idealforms-0.0.9/README.md
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 idealforms-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 idealforms-0.0.9/PKG-INFO
```

### Comparing `idealforms-0.0.2/.env.example` & `idealforms-0.0.9/.env.example`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/src/idealforms/bar.py` & `idealforms-0.0.9/src/idealforms/bar.py`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/src/idealforms/formatters.py` & `idealforms-0.0.9/src/idealforms/formatters.py`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/tests/bar_test.py` & `idealforms-0.0.9/tests/bar_test.py`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/tests/formatters_test.py` & `idealforms-0.0.9/tests/formatters_test.py`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/tests/bar_test_comparison_images/test_bar_out_labels.png` & `idealforms-0.0.9/tests/bar_test_comparison_images/test_bar_out_labels.png`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/tests/bar_test_comparison_images/test_bar_sort_alpha.png` & `idealforms-0.0.9/tests/bar_test_comparison_images/test_bar_sort_alpha.png`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/tests/bar_test_comparison_images/test_bar_sort_values.png` & `idealforms-0.0.9/tests/bar_test_comparison_images/test_bar_sort_values.png`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/LICENSE` & `idealforms-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/README.md` & `idealforms-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `idealforms-0.0.2/pyproject.toml` & `idealforms-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "idealforms"
-version = "0.0.2"
+version = "0.0.9"
 authors = [
   { name="Iain McConnell", email="buckler_08_matador@icloud.com" },
 ]
 description = "Some charts I prepared earlier"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `idealforms-0.0.2/PKG-INFO` & `idealforms-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idealforms
-Version: 0.0.2
+Version: 0.0.9
 Summary: Some charts I prepared earlier
 Project-URL: Homepage, https://github.com/ilmcconnell/idealforms
 Project-URL: Bug Tracker, https://github.com/ilmcconnell/idealforms/issues
 Author-email: Iain McConnell <buckler_08_matador@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

