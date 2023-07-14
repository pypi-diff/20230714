# Comparing `tmp/gocept.filestore-0.5.tar.gz` & `tmp/gocept.filestore-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocept.filestore-0.5.tar", last modified: Thu Mar 16 10:10:54 2023, max compression
+gzip compressed data, was "gocept.filestore-1.0.tar", last modified: Fri Jul 14 12:53:04 2023, max compression
```

## Comparing `gocept.filestore-0.5.tar` & `gocept.filestore-1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-16 10:10:54.049856 gocept.filestore-0.5/
--rw-r--r--   0 mac        (513) staff       (20)      123 2023-03-16 10:10:53.000000 gocept.filestore-0.5/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)      500 2023-03-16 10:10:53.000000 gocept.filestore-0.5/CHANGES.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-03-16 10:10:53.000000 gocept.filestore-0.5/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      178 2023-03-16 10:10:53.000000 gocept.filestore-0.5/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4317 2023-03-16 10:10:54.049994 gocept.filestore-0.5/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      134 2023-03-16 10:10:53.000000 gocept.filestore-0.5/README.md
--rw-r--r--   0 mac        (513) staff       (20)      213 2023-03-16 10:10:54.050581 gocept.filestore-0.5/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1977 2023-03-16 10:10:53.000000 gocept.filestore-0.5/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-16 10:10:54.042383 gocept.filestore-0.5/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-16 10:10:54.045543 gocept.filestore-0.5/src/gocept/
--rw-r--r--   0 mac        (513) staff       (20)       57 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-16 10:10:54.049574 gocept.filestore-0.5/src/gocept/filestore/
--rw-r--r--   0 mac        (513) staff       (20)     2560 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept/filestore/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      113 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept/filestore/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1524 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept/filestore/filestore.py
--rw-r--r--   0 mac        (513) staff       (20)      896 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept/filestore/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      203 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept/filestore/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-16 10:10:54.047798 gocept.filestore-0.5/src/gocept.filestore.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4317 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      586 2023-03-16 10:10:54.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       83 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2023-03-16 10:10:53.000000 gocept.filestore-0.5/src/gocept.filestore.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)      552 2023-03-16 10:10:53.000000 gocept.filestore-0.5/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:53:04.339490 gocept.filestore-1.0/
+-rw-r--r--   0 mac        (513) staff       (20)      123 2023-07-14 12:53:03.000000 gocept.filestore-1.0/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)      578 2023-07-14 12:53:03.000000 gocept.filestore-1.0/CHANGES.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-07-14 12:53:03.000000 gocept.filestore-1.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      178 2023-07-14 12:53:03.000000 gocept.filestore-1.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     4320 2023-07-14 12:53:04.339617 gocept.filestore-1.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      134 2023-07-14 12:53:03.000000 gocept.filestore-1.0/README.md
+-rw-r--r--   0 mac        (513) staff       (20)      213 2023-07-14 12:53:04.340093 gocept.filestore-1.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1910 2023-07-14 12:53:03.000000 gocept.filestore-1.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:53:04.332419 gocept.filestore-1.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:53:04.335385 gocept.filestore-1.0/src/gocept/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-07-14 12:53:03.000000 gocept.filestore-1.0/src/gocept/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:53:04.339208 gocept.filestore-1.0/src/gocept/filestore/
+-rw-r--r--   0 mac        (513) staff       (20)     2560 2023-07-14 12:53:03.000000 gocept.filestore-1.0/src/gocept/filestore/README.txt
+-rw-r--r--   0 mac        (513) staff       (20)      112 2023-07-14 12:53:03.000000 gocept.filestore-1.0/src/gocept/filestore/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1515 2023-07-14 12:53:03.000000 gocept.filestore-1.0/src/gocept/filestore/filestore.py
+-rw-r--r--   0 mac        (513) staff       (20)      895 2023-07-14 12:53:03.000000 gocept.filestore-1.0/src/gocept/filestore/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)      202 2023-07-14 12:53:03.000000 gocept.filestore-1.0/src/gocept/filestore/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:53:04.337637 gocept.filestore-1.0/src/gocept.filestore.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     4320 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      586 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       83 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-14 12:53:04.000000 gocept.filestore-1.0/src/gocept.filestore.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)      514 2023-07-14 12:53:03.000000 gocept.filestore-1.0/tox.ini
```

### Comparing `gocept.filestore-0.5/LICENSE.txt` & `gocept.filestore-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gocept.filestore-0.5/PKG-INFO` & `gocept.filestore-1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: gocept.filestore
-Version: 0.5
+Version: 1.0
 Summary: Provides maildir like access to files
 Home-page: https://github.com/gocept/gocept.filestore
 Author: gocept gmbh & co. kg
 Author-email: mail@gocept.com
 License: ZPL 2.1
 Keywords: filesystem consistency
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 .. contents::
 
 =========
 Filestore
@@ -153,14 +152,20 @@
 >>> shutil.rmtree(store_dir)
 
 
 =======
 Changes
 =======
 
+1.0 (2023-07-14)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 0.5 (2023-03-16)
 ================
 
 - Add support for Python 3,9, 3.10, 3.11.
 
 - Use GitHub actions as CI.
```

### Comparing `gocept.filestore-0.5/setup.py` & `gocept.filestore-1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 def read(*path):
     with open(os.path.join(*path)) as f:
         return f.read()
 
 
 setup(
     name='gocept.filestore',
-    version='0.5',
+    version='1.0',
     author='gocept gmbh & co. kg',
     author_email='mail@gocept.com',
     url='https://github.com/gocept/gocept.filestore',
     description="Provides maildir like access to files",
     long_description='.. contents::\n\n'
         + read(os.path.dirname(__file__), 'src', 'gocept', 'filestore',
                'README.txt')
         + '\n\n'
         + read('CHANGES.txt'),
     license="ZPL 2.1",
     classifiers=[
         'License :: OSI Approved',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Development Status :: 5 - Production/Stable',
@@ -44,14 +42,15 @@
             ],
     keywords='filesystem consistency',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     namespace_packages=['gocept'],
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.deferredimport',
         'zope.interface',
             ],
     extras_require={
         'test': [
```

### Comparing `gocept.filestore-0.5/src/gocept/filestore/README.txt` & `gocept.filestore-1.0/src/gocept/filestore/README.txt`

 * *Files identical despite different names*

### Comparing `gocept.filestore-0.5/src/gocept/filestore/filestore.py` & `gocept.filestore-1.0/src/gocept/filestore/filestore.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-
 import gocept.filestore.interfaces
 import os
 import os.path
 import shutil
 import zope.interface
 
 
 @zope.interface.implementer(gocept.filestore.interfaces.IFileStore)
-class FileStore(object):
+class FileStore:
 
     sub_dirs = ('tmp', 'new', 'cur')
 
     def __init__(self, path):
         self.path = path
 
     def prepare(self):
```

### Comparing `gocept.filestore-0.5/src/gocept/filestore/interfaces.py` & `gocept.filestore-1.0/src/gocept/filestore/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import zope.interface
 
 
 class IFileStore(zope.interface.Interface):
 
     def prepare():
         """Create the necessary directory structures."""
```

### Comparing `gocept.filestore-0.5/src/gocept.filestore.egg-info/PKG-INFO` & `gocept.filestore-1.0/src/gocept.filestore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: gocept.filestore
-Version: 0.5
+Version: 1.0
 Summary: Provides maildir like access to files
 Home-page: https://github.com/gocept/gocept.filestore
 Author: gocept gmbh & co. kg
 Author-email: mail@gocept.com
 License: ZPL 2.1
 Keywords: filesystem consistency
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 .. contents::
 
 =========
 Filestore
@@ -153,14 +152,20 @@
 >>> shutil.rmtree(store_dir)
 
 
 =======
 Changes
 =======
 
+1.0 (2023-07-14)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 0.5 (2023-03-16)
 ================
 
 - Add support for Python 3,9, 3.10, 3.11.
 
 - Use GitHub actions as CI.
```

### Comparing `gocept.filestore-0.5/src/gocept.filestore.egg-info/SOURCES.txt` & `gocept.filestore-1.0/src/gocept.filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocept.filestore-0.5/tox.ini` & `gocept.filestore-1.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [tox]
 envlist =
     flake8,
-    py27,
     py37,
     py38,
     py39,
     py310,
     py311,
     coverage,
 minversion = 1.6
@@ -17,15 +16,14 @@
 commands = zope-testrunner --test-path=src []
 
 [testenv:coverage]
 basepython = python3
 deps =
     {[testenv]deps}
     coverage
-    coverage-python-version
 commands =
     coverage run -m zope.testrunner --test-path=src
     coverage html
     coverage report -m
 
 [testenv:flake8]
 basepython = python3
```

