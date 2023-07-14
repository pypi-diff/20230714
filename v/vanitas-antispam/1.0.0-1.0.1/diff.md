# Comparing `tmp/vanitas-antispam-1.0.0.tar.gz` & `tmp/vanitas-antispam-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanitas-antispam-1.0.0.tar", last modified: Fri Jul 14 09:46:13 2023, max compression
+gzip compressed data, was "vanitas-antispam-1.0.1.tar", last modified: Fri Jul 14 09:55:07 2023, max compression
```

## Comparing `vanitas-antispam-1.0.0.tar` & `vanitas-antispam-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:46:13.308864 vanitas-antispam-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-14 09:46:01.000000 vanitas-antispam-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 09:46:13.308864 vanitas-antispam-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 09:46:01.000000 vanitas-antispam-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 09:46:01.000000 vanitas-antispam-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:46:13.308864 vanitas-antispam-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-14 09:46:01.000000 vanitas-antispam-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:46:13.308864 vanitas-antispam-1.0.0/vanitas-antispam/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-14 09:46:01.000000 vanitas-antispam-1.0.0/vanitas-antispam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:46:13.308864 vanitas-antispam-1.0.0/vanitas_antispam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 09:46:13.000000 vanitas-antispam-1.0.0/vanitas_antispam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 09:46:13.000000 vanitas-antispam-1.0.0/vanitas_antispam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:46:13.000000 vanitas-antispam-1.0.0/vanitas_antispam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 09:46:13.000000 vanitas-antispam-1.0.0/vanitas_antispam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 09:46:13.000000 vanitas-antispam-1.0.0/vanitas_antispam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:55:07.532503 vanitas-antispam-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-14 09:54:52.000000 vanitas-antispam-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 09:55:07.532503 vanitas-antispam-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 09:54:52.000000 vanitas-antispam-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 09:54:52.000000 vanitas-antispam-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:55:07.532503 vanitas-antispam-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-14 09:54:52.000000 vanitas-antispam-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:55:07.532503 vanitas-antispam-1.0.1/vanitas_antispam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 09:55:07.000000 vanitas-antispam-1.0.1/vanitas_antispam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-14 09:55:07.000000 vanitas-antispam-1.0.1/vanitas_antispam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:55:07.000000 vanitas-antispam-1.0.1/vanitas_antispam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 09:55:07.000000 vanitas-antispam-1.0.1/vanitas_antispam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 09:55:07.000000 vanitas-antispam-1.0.1/vanitas_antispam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:55:07.532503 vanitas-antispam-1.0.1/vanitaspy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-14 09:54:52.000000 vanitas-antispam-1.0.1/vanitaspy/__init__.py
```

### Comparing `vanitas-antispam-1.0.0/LICENSE` & `vanitas-antispam-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vanitas-antispam-1.0.0/PKG-INFO` & `vanitas-antispam-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanitas-antispam
-Version: 1.0.0
+Version: 1.0.1
 Summary: AntiSpam Wrapper for Vanitas
 Home-page: https://github.dev/ArshCypherZ/vanitaspy.git
 Author: ArshCypherZ
 Author-email: weebarsh@protonmail.com
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # How to use
 
 
 ```
-from vanitas-antispam import User
+from vanitaspy import User
 
 fk = User()
 
 x = fk.get_info(6040984893) # user id of telegram
 print(x)
 print(x.reason)
```

### Comparing `vanitas-antispam-1.0.0/setup.py` & `vanitas-antispam-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as txt:
     long_description = txt.read()
 
 setuptools.setup(
     name='vanitas-antispam',
-    version='1.0.0',
+    version='1.0.1',
     description='AntiSpam Wrapper for Vanitas',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='License :: OSI Approved :: MIT License',
     author='ArshCypherZ',
     author_email='weebarsh@protonmail.com',
     url='https://github.dev/ArshCypherZ/vanitaspy.git',
```

### Comparing `vanitas-antispam-1.0.0/vanitas-antispam/__init__.py` & `vanitas-antispam-1.0.1/vanitaspy/__init__.py`

 * *Files identical despite different names*

### Comparing `vanitas-antispam-1.0.0/vanitas_antispam.egg-info/PKG-INFO` & `vanitas-antispam-1.0.1/vanitas_antispam.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanitas-antispam
-Version: 1.0.0
+Version: 1.0.1
 Summary: AntiSpam Wrapper for Vanitas
 Home-page: https://github.dev/ArshCypherZ/vanitaspy.git
 Author: ArshCypherZ
 Author-email: weebarsh@protonmail.com
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # How to use
 
 
 ```
-from vanitas-antispam import User
+from vanitaspy import User
 
 fk = User()
 
 x = fk.get_info(6040984893) # user id of telegram
 print(x)
 print(x.reason)
```

