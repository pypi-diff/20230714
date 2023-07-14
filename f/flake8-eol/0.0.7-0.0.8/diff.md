# Comparing `tmp/flake8-eol-0.0.7.tar.gz` & `tmp/flake8-eol-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-eol-0.0.7.tar", last modified: Fri Jul 14 16:53:14 2023, max compression
+gzip compressed data, was "flake8-eol-0.0.8.tar", last modified: Fri Jul 14 18:59:44 2023, max compression
```

## Comparing `flake8-eol-0.0.7.tar` & `flake8-eol-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/
--rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      214 2023-07-14 16:14:24.000000 flake8-eol-0.0.7/README.md
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/flake8_eol/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      325 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       47 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/entry_points.txt
--rw-rw-r--   0 water     (1000) water     (1000)       14 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       11 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:42:38.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.py
--rw-rw-r--   0 water     (1000) water     (1000)      297 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:52:59.000000 flake8-eol-0.0.7/setup.py
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 18:59:44.254846 flake8-eol-0.0.8/
+-rw-rw-r--   0 water     (1000) water     (1000)     1055 2023-07-14 18:59:44.254846 flake8-eol-0.0.8/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      422 2023-07-14 18:58:00.000000 flake8-eol-0.0.8/README.md
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 18:59:44.254846 flake8-eol-0.0.8/flake8_eol/
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 18:59:44.254846 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/
+-rw-rw-r--   0 water     (1000) water     (1000)     1055 2023-07-14 18:59:44.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      325 2023-07-14 18:59:44.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/SOURCES.txt
+-rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 18:59:44.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/dependency_links.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       47 2023-07-14 18:59:44.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/entry_points.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       14 2023-07-14 18:59:44.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/requires.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       11 2023-07-14 18:59:44.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/top_level.txt
+-rw-rw-r--   0 water     (1000) water     (1000)      929 2023-07-14 18:53:58.000000 flake8-eol-0.0.8/flake8_eol/flake8_eol.py
+-rw-rw-r--   0 water     (1000) water     (1000)      297 2023-07-14 18:59:44.254846 flake8-eol-0.0.8/setup.cfg
+-rw-rw-r--   0 water     (1000) water     (1000)      736 2023-07-14 18:58:45.000000 flake8-eol-0.0.8/setup.py
```

### Comparing `flake8-eol-0.0.7/PKG-INFO` & `flake8-eol-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flake8-eol
-Version: 0.0.7
-Summary: Flake8 plugin to enforce EOL consistency
+Version: 0.0.8
+Summary: Flake8 plugin to enforce Unix/Linux EOL consistency
 Author: Claudio Scheer
 Author-email: claudioscheer@protonmail.com
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,14 +13,20 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # flake8-eol
 
-Flake8 plugin to enforce EOL consistency. The plugin simply checks if the first line of a file ends with '\r'. If do, it throws the warning EOL001.
+Flake8 plugin to enforce Unix/Linux EOL consistency. The plug-in simply checks that Python files' line endings are terminated with '\n' only.
+
+# Error codes
+
+| Error code | Description                                      |
+| :--------: | :----------------------------------------------- |
+|   EOL001   | Line endings are not consistent with Unix/Linux. |
 
 # Installation
 
 ```bash
 pip install flake8-eol
 ```
```

### Comparing `flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/PKG-INFO` & `flake8-eol-0.0.8/flake8_eol/flake8_eol.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flake8-eol
-Version: 0.0.7
-Summary: Flake8 plugin to enforce EOL consistency
+Version: 0.0.8
+Summary: Flake8 plugin to enforce Unix/Linux EOL consistency
 Author: Claudio Scheer
 Author-email: claudioscheer@protonmail.com
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,14 +13,20 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # flake8-eol
 
-Flake8 plugin to enforce EOL consistency. The plugin simply checks if the first line of a file ends with '\r'. If do, it throws the warning EOL001.
+Flake8 plugin to enforce Unix/Linux EOL consistency. The plug-in simply checks that Python files' line endings are terminated with '\n' only.
+
+# Error codes
+
+| Error code | Description                                      |
+| :--------: | :----------------------------------------------- |
+|   EOL001   | Line endings are not consistent with Unix/Linux. |
 
 # Installation
 
 ```bash
 pip install flake8-eol
 ```
```

### Comparing `flake8-eol-0.0.7/setup.py` & `flake8-eol-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 
 setup(
     name="flake8-eol",
-    version="0.0.7",
+    version="0.0.8",
     author="Claudio Scheer",
     author_email="claudioscheer@protonmail.com",
-    description="Flake8 plugin to enforce EOL consistency",
+    description="Flake8 plugin to enforce Unix/Linux EOL consistency",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Flake8",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

