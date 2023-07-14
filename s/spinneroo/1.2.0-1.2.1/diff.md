# Comparing `tmp/spinneroo-1.2.0.tar.gz` & `tmp/spinneroo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinneroo-1.2.0.tar", last modified: Wed Jul 12 13:52:44 2023, max compression
+gzip compressed data, was "spinneroo-1.2.1.tar", last modified: Fri Jul 14 15:51:09 2023, max compression
```

## Comparing `spinneroo-1.2.0.tar` & `spinneroo-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:52:44.681222 spinneroo-1.2.0/
--rw-rw-rw-   0        0        0       98 2023-07-12 13:52:44.000000 spinneroo-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2006 2023-07-12 13:52:44.681222 spinneroo-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1214 2023-07-01 08:57:02.000000 spinneroo-1.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.2.0/build.py
--rw-rw-rw-   0        0        0      630 2023-07-12 13:52:44.000000 spinneroo-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:52:44.681222 spinneroo-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1546 2023-07-12 13:52:20.000000 spinneroo-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:52:44.663201 spinneroo-1.2.0/spinneroo/
--rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.2.0/spinneroo/__init__.py
--rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.2.0/spinneroo/elements.py
--rw-rw-rw-   0        0        0    10309 2023-07-12 13:52:11.000000 spinneroo-1.2.0/spinneroo/progress.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:52:44.680223 spinneroo-1.2.0/spinneroo.egg-info/
--rw-rw-rw-   0        0        0     2006 2023-07-12 13:52:44.000000 spinneroo-1.2.0/spinneroo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-07-12 13:52:44.000000 spinneroo-1.2.0/spinneroo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:52:44.000000 spinneroo-1.2.0/spinneroo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-12 13:52:44.000000 spinneroo-1.2.0/spinneroo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 13:52:44.000000 spinneroo-1.2.0/spinneroo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 15:51:09.495419 spinneroo-1.2.1/
+-rw-rw-rw-   0        0        0       98 2023-07-14 15:51:09.000000 spinneroo-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2006 2023-07-14 15:51:09.495419 spinneroo-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1214 2023-07-01 08:57:02.000000 spinneroo-1.2.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 spinneroo-1.2.1/build.py
+-rw-rw-rw-   0        0        0      630 2023-07-14 15:51:09.000000 spinneroo-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-06-29 13:55:15.000000 spinneroo-1.2.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 21:50:48.000000 spinneroo-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:51:09.495419 spinneroo-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2023-07-14 15:50:57.000000 spinneroo-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:51:09.479906 spinneroo-1.2.1/spinneroo/
+-rw-rw-rw-   0        0        0       83 2023-06-15 21:53:50.000000 spinneroo-1.2.1/spinneroo/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-06-15 21:52:57.000000 spinneroo-1.2.1/spinneroo/elements.py
+-rw-rw-rw-   0        0        0    10312 2023-07-14 15:49:50.000000 spinneroo-1.2.1/spinneroo/progress.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:51:09.494418 spinneroo-1.2.1/spinneroo.egg-info/
+-rw-rw-rw-   0        0        0     2006 2023-07-14 15:51:09.000000 spinneroo-1.2.1/spinneroo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-07-14 15:51:09.000000 spinneroo-1.2.1/spinneroo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:51:09.000000 spinneroo-1.2.1/spinneroo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 15:51:09.000000 spinneroo-1.2.1/spinneroo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 15:51:09.000000 spinneroo-1.2.1/spinneroo.egg-info/top_level.txt
```

### Comparing `spinneroo-1.2.0/PKG-INFO` & `spinneroo-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 1.2.0
+Version: 1.2.1
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spinneroo-1.2.0/README.md` & `spinneroo-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spinneroo-1.2.0/build.py` & `spinneroo-1.2.1/build.py`

 * *Files identical despite different names*

### Comparing `spinneroo-1.2.0/pyproject.toml` & `spinneroo-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'spinneroo'
-version = '1.2.0'
+version = '1.2.1'
 description = 'A module for displaying progress messages and timers with spinners in the command line.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `spinneroo-1.2.0/setup.py` & `spinneroo-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='spinneroo',
-        version='1.2.0',
+        version='1.2.1',
         description=(
             "A module for displaying progress messages and "
             "timers with spinners in the command line."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `spinneroo-1.2.0/spinneroo/progress.py` & `spinneroo-1.2.1/spinneroo/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
         :return: The status value
         """
 
         self.stop()
 
         if exception is not None:
-            return False
+            raise exception
         # end if
 
         return True
     # end __exit__
 
     @property
     def paused(self) -> bool:
```

### Comparing `spinneroo-1.2.0/spinneroo.egg-info/PKG-INFO` & `spinneroo-1.2.1/spinneroo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinneroo
-Version: 1.2.0
+Version: 1.2.1
 Summary: A module for displaying progress messages and timers with spinners in the command line.
 Home-page: https://github.com/Shahaf-F-S/spinneroo
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

