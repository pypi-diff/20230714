# Comparing `tmp/pypdtools-0.0.4.tar.gz` & `tmp/pypdtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdtools-0.0.4.tar", last modified: Mon Jul  3 17:34:58 2023, max compression
+gzip compressed data, was "pypdtools-0.0.5.tar", last modified: Fri Jul 14 18:50:26 2023, max compression
```

## Comparing `pypdtools-0.0.4.tar` & `pypdtools-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.567193 pypdtools-0.0.4/
--rw-rw-rw-   0        0        0     1511 2023-06-28 17:19:48.000000 pypdtools-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2518 2023-07-03 17:34:58.567193 pypdtools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1850 2023-06-30 15:40:55.000000 pypdtools-0.0.4/README.md
--rw-rw-rw-   0        0        0     1847 2023-07-03 17:34:08.000000 pypdtools-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 17:34:58.568194 pypdtools-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.534186 pypdtools-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.540189 pypdtools-0.0.4/src/pypdtools/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.559192 pypdtools-0.0.4/src/pypdtools/abc/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/abc/__init__.py
--rw-rw-rw-   0        0        0      677 2023-06-28 21:28:40.000000 pypdtools-0.0.4/src/pypdtools/abc/dataframe.py
--rw-rw-rw-   0        0        0      709 2023-06-30 15:31:22.000000 pypdtools-0.0.4/src/pypdtools/abc/scripts.py
--rw-rw-rw-   0        0        0      430 2023-07-03 16:45:32.000000 pypdtools-0.0.4/src/pypdtools/abc/services.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.562192 pypdtools-0.0.4/src/pypdtools/core/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/core/__init__.py
--rw-rw-rw-   0        0        0     6568 2023-06-30 15:31:22.000000 pypdtools-0.0.4/src/pypdtools/core/dataframe.py
--rw-rw-rw-   0        0        0     2627 2023-06-30 15:31:22.000000 pypdtools-0.0.4/src/pypdtools/core/scripts.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.564193 pypdtools-0.0.4/src/pypdtools/core/services/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/core/services/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-07-03 16:45:32.000000 pypdtools-0.0.4/src/pypdtools/core/services/load_services.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.566193 pypdtools-0.0.4/src/pypdtools/utils/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.4/src/pypdtools/utils/__init__.py
--rw-rw-rw-   0        0        0     2207 2023-06-30 14:41:49.000000 pypdtools-0.0.4/src/pypdtools/utils/asyncs.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:34:58.555191 pypdtools-0.0.4/src/pypdtools.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      249 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 17:34:58.000000 pypdtools-0.0.4/src/pypdtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.064479 pypdtools-0.0.5/
+-rw-rw-rw-   0        0        0     1511 2023-06-28 17:19:48.000000 pypdtools-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2518 2023-07-14 18:50:26.063478 pypdtools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1850 2023-06-30 15:40:55.000000 pypdtools-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1847 2023-07-14 18:49:35.000000 pypdtools-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 18:50:26.064479 pypdtools-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.006954 pypdtools-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.023961 pypdtools-0.0.5/src/pypdtools/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.5/src/pypdtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.051476 pypdtools-0.0.5/src/pypdtools/abc/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.5/src/pypdtools/abc/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-06-28 21:28:40.000000 pypdtools-0.0.5/src/pypdtools/abc/dataframe.py
+-rw-rw-rw-   0        0        0      709 2023-06-30 15:31:22.000000 pypdtools-0.0.5/src/pypdtools/abc/scripts.py
+-rw-rw-rw-   0        0        0      430 2023-07-03 16:45:32.000000 pypdtools-0.0.5/src/pypdtools/abc/services.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.056477 pypdtools-0.0.5/src/pypdtools/core/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.5/src/pypdtools/core/__init__.py
+-rw-rw-rw-   0        0        0     6568 2023-06-30 15:31:22.000000 pypdtools-0.0.5/src/pypdtools/core/dataframe.py
+-rw-rw-rw-   0        0        0     2626 2023-07-14 18:48:03.000000 pypdtools-0.0.5/src/pypdtools/core/scripts.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.058477 pypdtools-0.0.5/src/pypdtools/core/services/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.5/src/pypdtools/core/services/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-07-03 16:45:32.000000 pypdtools-0.0.5/src/pypdtools/core/services/load_services.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.061478 pypdtools-0.0.5/src/pypdtools/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.5/src/pypdtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-06-30 14:41:49.000000 pypdtools-0.0.5/src/pypdtools/utils/asyncs.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:50:26.046475 pypdtools-0.0.5/src/pypdtools.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-07-14 18:50:25.000000 pypdtools-0.0.5/src/pypdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-07-14 18:50:26.000000 pypdtools-0.0.5/src/pypdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:50:25.000000 pypdtools-0.0.5/src/pypdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      249 2023-07-14 18:50:25.000000 pypdtools-0.0.5/src/pypdtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 18:50:25.000000 pypdtools-0.0.5/src/pypdtools.egg-info/top_level.txt
```

### Comparing `pypdtools-0.0.4/LICENSE` & `pypdtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/PKG-INFO` & `pypdtools-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package with tools for pandas
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>
 Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/
 Project-URL: Bug Tracker, https://github.com/msbar/pypdtools/issues
 Keywords: pandas,tools,asyncio
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypdtools Version: 0.0.4 Summary: Package with
+Metadata-Version: 2.1 Name: pypdtools Version: 0.0.5 Summary: Package with
 tools for pandas Author-email: Marciel Barcellos
 barcellos@tcmrio.tc.br> Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/ Project-URL: Bug
 Tracker, https://github.com/msbar/pypdtools/issues Keywords:
 pandas,tools,asyncio Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `pypdtools-0.0.4/README.md` & `pypdtools-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/pyproject.toml` & `pypdtools-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "pypdtools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Marciel Barcellos", email="marciel.barcellos@tcmrio.tc.br" }
 ]
 description = "Package with tools for pandas"
 
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pypdtools-0.0.4/src/pypdtools/abc/dataframe.py` & `pypdtools-0.0.5/src/pypdtools/abc/dataframe.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/src/pypdtools/abc/scripts.py` & `pypdtools-0.0.5/src/pypdtools/abc/scripts.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/src/pypdtools/core/dataframe.py` & `pypdtools-0.0.5/src/pypdtools/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/src/pypdtools/core/scripts.py` & `pypdtools-0.0.5/src/pypdtools/core/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class BaseEtl(AbstractEtl):
     """This class is used to create an ETL object."""
 
     def __init__(self) -> None:
         """This method is used to initialize the ETL object."""
         super().__init__()
-        self.data = None
+        self._df = None
         self.executed = False
 
     def extract(self):
         """This method is used to get data from the source."""
         raise NotImplementedError
 
     def transform(self):
```

### Comparing `pypdtools-0.0.4/src/pypdtools/core/services/load_services.py` & `pypdtools-0.0.5/src/pypdtools/core/services/load_services.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/src/pypdtools/utils/asyncs.py` & `pypdtools-0.0.5/src/pypdtools/utils/asyncs.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.4/src/pypdtools.egg-info/PKG-INFO` & `pypdtools-0.0.5/src/pypdtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package with tools for pandas
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>
 Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/
 Project-URL: Bug Tracker, https://github.com/msbar/pypdtools/issues
 Keywords: pandas,tools,asyncio
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypdtools Version: 0.0.4 Summary: Package with
+Metadata-Version: 2.1 Name: pypdtools Version: 0.0.5 Summary: Package with
 tools for pandas Author-email: Marciel Barcellos
 barcellos@tcmrio.tc.br> Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/ Project-URL: Bug
 Tracker, https://github.com/msbar/pypdtools/issues Keywords:
 pandas,tools,asyncio Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `pypdtools-0.0.4/src/pypdtools.egg-info/SOURCES.txt` & `pypdtools-0.0.5/src/pypdtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

