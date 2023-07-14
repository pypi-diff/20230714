# Comparing `tmp/USSCameraTools-0.1.0.tar.gz` & `tmp/USSCameraTools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "USSCameraTools-0.1.0.tar", last modified: Fri Oct 21 18:14:01 2022, max compression
+gzip compressed data, was "USSCameraTools-0.1.1.tar", last modified: Fri Jul 14 19:16:48 2023, max compression
```

## Comparing `USSCameraTools-0.1.0.tar` & `USSCameraTools-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-10-21 18:14:01.429603 USSCameraTools-0.1.0/
--rw-rw-rw-   0        0        0      706 2022-10-21 18:14:01.428626 USSCameraTools-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-21 18:14:01.401290 USSCameraTools-0.1.0/USSCameraTools/
--rw-rw-rw-   0        0        0       64 2022-10-21 18:13:54.000000 USSCameraTools-0.1.0/USSCameraTools/__init__.py
--rw-rw-rw-   0        0        0     3704 2022-10-20 20:24:03.000000 USSCameraTools-0.1.0/USSCameraTools/core.py
-drwxrwxrwx   0        0        0        0 2022-10-21 18:14:01.427650 USSCameraTools-0.1.0/USSCameraTools.egg-info/
--rw-rw-rw-   0        0        0      706 2022-10-21 18:14:01.000000 USSCameraTools-0.1.0/USSCameraTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2022-10-21 18:14:01.000000 USSCameraTools-0.1.0/USSCameraTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-21 18:14:01.000000 USSCameraTools-0.1.0/USSCameraTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-10-21 18:14:01.000000 USSCameraTools-0.1.0/USSCameraTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-10-21 18:14:01.000000 USSCameraTools-0.1.0/USSCameraTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-21 18:14:01.429603 USSCameraTools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      876 2022-10-21 18:13:27.000000 USSCameraTools-0.1.0/setup.py
+drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)      945 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/PKG-INFO
+drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/USSCameraTools/
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       58 2023-07-14 17:24:01.000000 USSCameraTools-0.1.1/USSCameraTools/__init__.py
+drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/USSCameraTools.egg-info/
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)      945 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/PKG-INFO
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)      224 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)        1 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       25 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/requires.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       15 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/top_level.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       38 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/setup.cfg
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)     1101 2023-07-14 19:16:46.000000 USSCameraTools-0.1.1/setup.py
```

### Comparing `USSCameraTools-0.1.0/setup.py` & `USSCameraTools-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from setuptools import setup,find_packages
-
-setup(
-    name='USSCameraTools',
-    version='0.1.0',    
-    description='A example Python package',
-    url='https://github.com/USSVision/USSCommonTools/tree/main/Packages/USSCameraTools',
-    author='USS Vision',
-    author_email='bhelfer@ussvision.com',
-    license='MIT',
-    packages=find_packages(),
-    install_requires=['wheel','opencv-python','harvesters',],
-
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: MIT License',  
-        'Operating System :: POSIX :: Linux',
-        'Operating System :: Microsoft :: Windows :: Windows 10',         
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-)
+from setuptools import setup
+
+setup(
+    name='USSCameraTools',
+    version='0.1.1',
+    description='USSCamera: Python package for interacting with GigE cameras using the Harvesters library',
+    long_description='USSCamera is a Python package that provides functionality to interact with GigE cameras using the Harvesters library. It allows you to easily connect to cameras, capture images, trigger the camera, and retrieve camera attributes.',
+    long_description_content_type='text/markdown',
+    author='USSVision',
+    author_email='bhelfer@ussvision.com',
+    packages=['USSCameraTools'],
+    install_requires=[
+        'harvesters',
+        'opencv-python',
+    ],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: Microsoft :: Windows :: Windows 10',
+        'Operating System :: POSIX :: Linux',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
+    ],
+)
```

