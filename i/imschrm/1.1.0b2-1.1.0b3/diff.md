# Comparing `tmp/imschrm-1.1.0b2.tar.gz` & `tmp/imschrm-1.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Z:\projects\imsc-hrm\imschrm-repo\dist\.tmp-4ob2aoh1\imschrm-1.1.0b2.tar", last modified: Thu Jul 13 21:55:11 2023, max compression
+gzip compressed data, was "Z:\projects\imsc-hrm\imschrm-repo\dist\.tmp-jw1dnv3h\imschrm-1.1.0b3.tar", last modified: Thu Jul 13 21:58:14 2023, max compression
```

## Comparing `imschrm-1.1.0b2.tar` & `imschrm-1.1.0b3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.118954 imschrm-1.1.0b2/
--rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0b2/LICENSE.txt
--rw-rw-rw-   0        0        0     2981 2023-07-13 21:55:12.583696 imschrm-1.1.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     2068 2023-06-22 15:26:04.000000 imschrm-1.1.0b2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 21:55:12.589709 imschrm-1.1.0b2/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-07-13 21:54:13.000000 imschrm-1.1.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.043732 imschrm-1.1.0b2/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.049764 imschrm-1.1.0b2/src/main/
-drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.053793 imschrm-1.1.0b2/src/main/python/
-drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.351091 imschrm-1.1.0b2/src/main/python/imschrm/
--rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0b2/src/main/python/imschrm/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-07-13 17:28:11.000000 imschrm-1.1.0b2/src/main/python/imschrm/cli.py
--rw-rw-rw-   0        0        0   366016 2022-04-06 16:51:28.000000 imschrm-1.1.0b2/src/main/python/imschrm/codepoint_sets.py
--rw-rw-rw-   0        0        0     3394 2021-06-02 18:29:37.000000 imschrm-1.1.0b2/src/main/python/imschrm/doc_sequence.py
--rw-rw-rw-   0        0        0    12174 2023-07-13 17:28:31.000000 imschrm-1.1.0b2/src/main/python/imschrm/hrm.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:55:12.222209 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-07-13 21:55:12.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 21:55:11.000000 imschrm-1.1.0b2/src/main/python/imschrm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 21:58:15.094869 imschrm-1.1.0b3/
+-rw-rw-rw-   0        0        0     1260 2021-06-02 18:29:36.000000 imschrm-1.1.0b3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2981 2023-07-13 21:58:15.578155 imschrm-1.1.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     2068 2023-06-22 15:26:04.000000 imschrm-1.1.0b3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 21:58:15.584172 imschrm-1.1.0b3/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2023-07-13 21:58:02.000000 imschrm-1.1.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:58:15.041725 imschrm-1.1.0b3/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:58:15.045737 imschrm-1.1.0b3/src/main/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:58:15.049747 imschrm-1.1.0b3/src/main/python/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:58:15.305426 imschrm-1.1.0b3/src/main/python/imschrm/
+-rw-rw-rw-   0        0        0        0 2021-06-02 18:29:28.000000 imschrm-1.1.0b3/src/main/python/imschrm/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-07-13 21:57:46.000000 imschrm-1.1.0b3/src/main/python/imschrm/cli.py
+-rw-rw-rw-   0        0        0   366016 2022-04-06 16:51:28.000000 imschrm-1.1.0b3/src/main/python/imschrm/codepoint_sets.py
+-rw-rw-rw-   0        0        0     3394 2021-06-02 18:29:37.000000 imschrm-1.1.0b3/src/main/python/imschrm/doc_sequence.py
+-rw-rw-rw-   0        0        0    12174 2023-07-13 21:57:46.000000 imschrm-1.1.0b3/src/main/python/imschrm/hrm.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:58:15.224215 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-07-13 21:58:14.000000 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-07-13 21:58:15.000000 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:58:14.000000 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-13 21:58:14.000000 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-13 21:58:14.000000 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 21:58:14.000000 imschrm-1.1.0b3/src/main/python/imschrm.egg-info/top_level.txt
```

### Comparing `imschrm-1.1.0b2/LICENSE.txt` & `imschrm-1.1.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b2/PKG-INFO` & `imschrm-1.1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imschrm
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: Validates IMSC documents against the IMSC HRM
 Home-page: https://www.sandflow.com
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/imscHRM/issues
 Project-URL: Source, https://github.com/sandflow/imscHRM
 Keywords: ttml,imsc,smpte-tt,hrm,complexity
```

### Comparing `imschrm-1.1.0b2/README.md` & `imschrm-1.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b2/setup.py` & `imschrm-1.1.0b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setup(
-  name='imschrm', 
-  version='1.1.0b2',
+  name='imschrm',
+  version='1.1.0b3',
   description='Validates IMSC documents against the IMSC HRM',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Sandflow Consulting LLC',
   author_email='info@sandflow.com',
   url='https://www.sandflow.com',
   project_urls={
```

### Comparing `imschrm-1.1.0b2/src/main/python/imschrm/cli.py` & `imschrm-1.1.0b3/src/main/python/imschrm/cli.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b2/src/main/python/imschrm/codepoint_sets.py` & `imschrm-1.1.0b3/src/main/python/imschrm/codepoint_sets.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b2/src/main/python/imschrm/doc_sequence.py` & `imschrm-1.1.0b3/src/main/python/imschrm/doc_sequence.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b2/src/main/python/imschrm/hrm.py` & `imschrm-1.1.0b3/src/main/python/imschrm/hrm.py`

 * *Files identical despite different names*

### Comparing `imschrm-1.1.0b2/src/main/python/imschrm.egg-info/PKG-INFO` & `imschrm-1.1.0b3/src/main/python/imschrm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imschrm
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: Validates IMSC documents against the IMSC HRM
 Home-page: https://www.sandflow.com
 Author: Sandflow Consulting LLC
 Author-email: info@sandflow.com
 Project-URL: Bug Reports, https://github.com/sandflow/imscHRM/issues
 Project-URL: Source, https://github.com/sandflow/imscHRM
 Keywords: ttml,imsc,smpte-tt,hrm,complexity
```

### Comparing `imschrm-1.1.0b2/src/main/python/imschrm.egg-info/SOURCES.txt` & `imschrm-1.1.0b3/src/main/python/imschrm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

