# Comparing `tmp/pyhandytools-0.0.6.tar.gz` & `tmp/pyhandytools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhandytools-0.0.6.tar", last modified: Fri Jul 14 16:22:03 2023, max compression
+gzip compressed data, was "pyhandytools-0.0.7.tar", last modified: Fri Jul 14 16:33:06 2023, max compression
```

## Comparing `pyhandytools-0.0.6.tar` & `pyhandytools-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:22:03.053615 pyhandytools-0.0.6/
--rw-r--r--   0 jmchen     (501) staff       (20)    11354 2023-06-24 15:27:46.000000 pyhandytools-0.0.6/LICENSE
--rw-r--r--   0 jmchen     (501) staff       (20)      633 2023-07-14 16:22:03.053435 pyhandytools-0.0.6/PKG-INFO
--rw-r--r--   0 jmchen     (501) staff       (20)      202 2023-06-30 16:53:05.000000 pyhandytools-0.0.6/README.md
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:22:03.052461 pyhandytools-0.0.6/pyhandytools/
--rw-r--r--   0 jmchen     (501) staff       (20)       48 2023-06-24 15:16:23.000000 pyhandytools-0.0.6/pyhandytools/__init__.py
--rw-r--r--   0 jmchen     (501) staff       (20)      237 2023-07-14 16:08:13.000000 pyhandytools-0.0.6/pyhandytools/env.py
--rw-r--r--   0 jmchen     (501) staff       (20)     1661 2023-07-14 16:08:13.000000 pyhandytools-0.0.6/pyhandytools/file.py
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:22:03.053241 pyhandytools-0.0.6/pyhandytools.egg-info/
--rw-r--r--   0 jmchen     (501) staff       (20)      633 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/PKG-INFO
--rw-r--r--   0 jmchen     (501) staff       (20)      271 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/SOURCES.txt
--rw-r--r--   0 jmchen     (501) staff       (20)        1 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/dependency_links.txt
--rw-r--r--   0 jmchen     (501) staff       (20)        7 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/requires.txt
--rw-r--r--   0 jmchen     (501) staff       (20)       13 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/top_level.txt
--rw-r--r--   0 jmchen     (501) staff       (20)       38 2023-07-14 16:22:03.053668 pyhandytools-0.0.6/setup.cfg
--rw-r--r--   0 jmchen     (501) staff       (20)      938 2023-07-14 16:21:48.000000 pyhandytools-0.0.6/setup.py
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:33:06.142387 pyhandytools-0.0.7/
+-rw-r--r--   0 jmchen     (501) staff       (20)     1069 2023-07-14 16:28:56.000000 pyhandytools-0.0.7/LICENSE
+-rw-r--r--   0 jmchen     (501) staff       (20)      633 2023-07-14 16:33:06.142224 pyhandytools-0.0.7/PKG-INFO
+-rw-r--r--   0 jmchen     (501) staff       (20)      202 2023-06-30 16:53:05.000000 pyhandytools-0.0.7/README.md
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:33:06.140951 pyhandytools-0.0.7/pyhandytools/
+-rw-r--r--   0 jmchen     (501) staff       (20)       48 2023-06-24 15:16:23.000000 pyhandytools-0.0.7/pyhandytools/__init__.py
+-rw-r--r--   0 jmchen     (501) staff       (20)      237 2023-07-14 16:08:13.000000 pyhandytools-0.0.7/pyhandytools/env.py
+-rw-r--r--   0 jmchen     (501) staff       (20)     1661 2023-07-14 16:08:13.000000 pyhandytools-0.0.7/pyhandytools/file.py
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:33:06.142039 pyhandytools-0.0.7/pyhandytools.egg-info/
+-rw-r--r--   0 jmchen     (501) staff       (20)      633 2023-07-14 16:33:06.000000 pyhandytools-0.0.7/pyhandytools.egg-info/PKG-INFO
+-rw-r--r--   0 jmchen     (501) staff       (20)      271 2023-07-14 16:33:06.000000 pyhandytools-0.0.7/pyhandytools.egg-info/SOURCES.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)        1 2023-07-14 16:33:06.000000 pyhandytools-0.0.7/pyhandytools.egg-info/dependency_links.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)        7 2023-07-14 16:33:06.000000 pyhandytools-0.0.7/pyhandytools.egg-info/requires.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)       13 2023-07-14 16:33:06.000000 pyhandytools-0.0.7/pyhandytools.egg-info/top_level.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)       38 2023-07-14 16:33:06.142436 pyhandytools-0.0.7/setup.cfg
+-rw-r--r--   0 jmchen     (501) staff       (20)      867 2023-07-14 16:32:55.000000 pyhandytools-0.0.7/setup.py
```

### Comparing `pyhandytools-0.0.6/PKG-INFO` & `pyhandytools-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhandytools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python handy tools
 Home-page: https://github.com/JimouChen/py-handy
 Author: Jimou Chen
 Author-email: jmchen1024@gmail.com
 Keywords: toolbox,kit,utils,tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyhandytools-0.0.6/pyhandytools/file.py` & `pyhandytools-0.0.7/pyhandytools/file.py`

 * *Files identical despite different names*

### Comparing `pyhandytools-0.0.6/pyhandytools.egg-info/PKG-INFO` & `pyhandytools-0.0.7/pyhandytools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhandytools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python handy tools
 Home-page: https://github.com/JimouChen/py-handy
 Author: Jimou Chen
 Author-email: jmchen1024@gmail.com
 Keywords: toolbox,kit,utils,tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyhandytools-0.0.6/setup.py` & `pyhandytools-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from setuptools import setup, find_packages
 
 with open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyhandytools',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     include_package_data=True,
     url='https://github.com/JimouChen/py-handy',
     author='Jimou Chen',
     author_email='jmchen1024@gmail.com',
     description='Python handy tools',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['toolbox', 'kit', 'utils', 'tools'],
-    classifiers=[  # 指定该库依赖的Python版本、license、操作系统之类的
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'loguru'
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

