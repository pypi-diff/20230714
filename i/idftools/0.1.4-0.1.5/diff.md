# Comparing `tmp/idftools-0.1.4.tar.gz` & `tmp/idftools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idftools-0.1.4.tar", last modified: Fri Jul 14 16:37:52 2023, max compression
+gzip compressed data, was "idftools-0.1.5.tar", last modified: Fri Jul 14 19:47:12 2023, max compression
```

## Comparing `idftools-0.1.4.tar` & `idftools-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 16:37:52.343838 idftools-0.1.4/
--rw-rw-r--   0 enio      (1000) enio      (1000)      668 2023-07-14 16:37:52.343838 idftools-0.1.4/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      249 2023-07-14 14:44:57.000000 idftools-0.1.4/README.md
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 16:37:52.343838 idftools-0.1.4/idftools/
--rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.4/idftools/certificate.py
--rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.4/idftools/driversfactory.py
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 16:37:52.343838 idftools-0.1.4/idftools/idftools.egg-info/
--rw-rw-r--   0 enio      (1000) enio      (1000)      668 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/SOURCES.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/dependency_links.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)      353 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/requires.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/top_level.txt
--rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.4/idftools/utilities.py
--rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 16:37:52.343838 idftools-0.1.4/setup.cfg
--rw-rw-r--   0 enio      (1000) enio      (1000)      819 2023-07-14 16:37:45.000000 idftools-0.1.4/setup.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 19:47:12.943990 idftools-0.1.5/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     5869 2023-07-14 19:47:12.939990 idftools-0.1.5/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)     3909 2023-07-14 19:46:57.000000 idftools-0.1.5/README.md
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 19:47:12.939990 idftools-0.1.5/idftools/
+-rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.5/idftools/certificate.py
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.5/idftools/driversfactory.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 19:47:12.939990 idftools-0.1.5/idftools/idftools.egg-info/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     5869 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)      373 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/requires.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/top_level.txt
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.5/idftools/utilities.py
+-rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 19:47:12.943990 idftools-0.1.5/setup.cfg
+-rw-rw-r--   0 enio      (1000) enio      (1000)      917 2023-07-14 19:45:21.000000 idftools-0.1.5/setup.py
```

### Comparing `idftools-0.1.4/idftools/certificate.py` & `idftools-0.1.5/idftools/certificate.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.4/idftools/driversfactory.py` & `idftools-0.1.5/idftools/driversfactory.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.4/idftools/utilities.py` & `idftools-0.1.5/idftools/utilities.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.4/setup.py` & `idftools-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,25 @@
     requirements = ''
 
 print(f'requirements={requirements}')
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+print(f'long_description={long_description}')
+
 setup(
+    version="0.1.5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=requirements,
     name="idftools",
     author_email="eniodefarias@gmail.com",
     author="eniodefarias",
-    version="0.1.4",
-    url="http://ideiadofuturo.com.br/pypi",
+    url="https://github.com/eniodefarias/pypi-idftools",
     description="Um pacote com alguns utilitarios uteis",
     py_modules=["utilities", "driversfactory", "certificate"],
     package_dir={"": "idftools"}
 )
 
-# .venv/bin/python3 setup.py sdist bdist_wheel
+# .venv/bin/python3 setup.py sdist bdist_wheel
+# twine upload --skip-existing dist/*
```

