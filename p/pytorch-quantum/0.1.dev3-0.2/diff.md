# Comparing `tmp/pytorch-quantum-0.1.dev3.tar.gz` & `tmp/pytorch-quantum-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytorch-quantum-0.1.dev3.tar", last modified: Wed Dec 23 14:19:17 2020, max compression
+gzip compressed data, was "pytorch-quantum-0.2.tar", last modified: Fri Jul 14 12:37:53 2023, max compression
```

## Comparing `pytorch-quantum-0.1.dev3.tar` & `pytorch-quantum-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 14:19:17.526378 pytorch-quantum-0.1.dev3/
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-23 14:18:54.000000 pytorch-quantum-0.1.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1355 2020-12-23 14:19:17.526378 pytorch-quantum-0.1.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      517 2020-12-23 14:18:54.000000 pytorch-quantum-0.1.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 14:19:17.522378 pytorch-quantum-0.1.dev3/pytorch_quantum/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-23 14:18:54.000000 pytorch-quantum-0.1.dev3/pytorch_quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 14:19:17.526378 pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1355 2020-12-23 14:19:17.000000 pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      252 2020-12-23 14:19:17.000000 pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-23 14:19:17.000000 pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       65 2020-12-23 14:19:17.000000 pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-12-23 14:19:17.000000 pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-23 14:19:17.526378 pytorch-quantum-0.1.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1094 2020-12-23 14:18:54.000000 pytorch-quantum-0.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:53.863672 pytorch-quantum-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 12:37:49.000000 pytorch-quantum-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 12:37:53.863672 pytorch-quantum-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 12:37:49.000000 pytorch-quantum-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:53.863672 pytorch-quantum-0.2/pytorch_quantum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:49.000000 pytorch-quantum-0.2/pytorch_quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:53.863672 pytorch-quantum-0.2/pytorch_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 12:37:53.000000 pytorch-quantum-0.2/pytorch_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 12:37:53.000000 pytorch-quantum-0.2/pytorch_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:37:53.000000 pytorch-quantum-0.2/pytorch_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 12:37:53.000000 pytorch-quantum-0.2/pytorch_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 12:37:53.000000 pytorch-quantum-0.2/pytorch_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:37:53.863672 pytorch-quantum-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-14 12:37:49.000000 pytorch-quantum-0.2/setup.py
```

### Comparing `pytorch-quantum-0.1.dev3/PKG-INFO` & `pytorch-quantum-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pytorch-quantum
-Version: 0.1.dev3
+Version: 0.2
 Summary: A PyTorch based library for Quantum Machine Learning
 Home-page: http://github.com/pytorch-quantum
 Author-email: contact@anuragsaharoy.me
 License: UNKNOWN
-Description: ![](docs/source/_static/pytorch-quantum-logo.png)
-        
-        # pytorch-quantum: Build Quantum Machine Learning models leveraging the power of the PyTorch ecosystem
-        
-        [![PyPI version fury.io](https://badge.fury.io/py/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
-        [![PyPI license](https://img.shields.io/pypi/l/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+
+![](docs/source/_static/pytorch-quantum-logo.png)
+
+# pytorch-quantum: Quantum Dynamics simulation with PyTorch
+
+[![PyPI version fury.io](https://badge.fury.io/py/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
+[![PyPI license](https://img.shields.io/pypi/l/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
+
```

### Comparing `pytorch-quantum-0.1.dev3/pytorch_quantum.egg-info/PKG-INFO` & `pytorch-quantum-0.2/pytorch_quantum.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pytorch-quantum
-Version: 0.1.dev3
+Version: 0.2
 Summary: A PyTorch based library for Quantum Machine Learning
 Home-page: http://github.com/pytorch-quantum
 Author-email: contact@anuragsaharoy.me
 License: UNKNOWN
-Description: ![](docs/source/_static/pytorch-quantum-logo.png)
-        
-        # pytorch-quantum: Build Quantum Machine Learning models leveraging the power of the PyTorch ecosystem
-        
-        [![PyPI version fury.io](https://badge.fury.io/py/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
-        [![PyPI license](https://img.shields.io/pypi/l/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+
+![](docs/source/_static/pytorch-quantum-logo.png)
+
+# pytorch-quantum: Quantum Dynamics simulation with PyTorch
+
+[![PyPI version fury.io](https://badge.fury.io/py/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
+[![PyPI license](https://img.shields.io/pypi/l/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytorch-quantum.svg)](https://pypi.python.org/pypi/pytorch-quantum/)
+
```

