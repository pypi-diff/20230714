# Comparing `tmp/pyhandytools-0.0.5.tar.gz` & `tmp/pyhandytools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhandytools-0.0.5.tar", last modified: Fri Jul 14 16:09:45 2023, max compression
+gzip compressed data, was "pyhandytools-0.0.6.tar", last modified: Fri Jul 14 16:22:03 2023, max compression
```

## Comparing `pyhandytools-0.0.5.tar` & `pyhandytools-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:09:45.420569 pyhandytools-0.0.5/
--rw-r--r--   0 jmchen     (501) staff       (20)    11354 2023-06-24 15:27:46.000000 pyhandytools-0.0.5/LICENSE
--rw-r--r--   0 jmchen     (501) staff       (20)      487 2023-07-14 16:09:45.420375 pyhandytools-0.0.5/PKG-INFO
--rw-r--r--   0 jmchen     (501) staff       (20)      202 2023-06-30 16:53:05.000000 pyhandytools-0.0.5/README.md
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:09:45.419138 pyhandytools-0.0.5/pyhandytools/
--rw-r--r--   0 jmchen     (501) staff       (20)       48 2023-06-24 15:16:23.000000 pyhandytools-0.0.5/pyhandytools/__init__.py
--rw-r--r--   0 jmchen     (501) staff       (20)      237 2023-07-14 16:08:13.000000 pyhandytools-0.0.5/pyhandytools/env.py
--rw-r--r--   0 jmchen     (501) staff       (20)     1661 2023-07-14 16:08:13.000000 pyhandytools-0.0.5/pyhandytools/file.py
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:09:45.420151 pyhandytools-0.0.5/pyhandytools.egg-info/
--rw-r--r--   0 jmchen     (501) staff       (20)      487 2023-07-14 16:09:45.000000 pyhandytools-0.0.5/pyhandytools.egg-info/PKG-INFO
--rw-r--r--   0 jmchen     (501) staff       (20)      271 2023-07-14 16:09:45.000000 pyhandytools-0.0.5/pyhandytools.egg-info/SOURCES.txt
--rw-r--r--   0 jmchen     (501) staff       (20)        1 2023-07-14 16:09:45.000000 pyhandytools-0.0.5/pyhandytools.egg-info/dependency_links.txt
--rw-r--r--   0 jmchen     (501) staff       (20)        7 2023-07-14 16:09:45.000000 pyhandytools-0.0.5/pyhandytools.egg-info/requires.txt
--rw-r--r--   0 jmchen     (501) staff       (20)       13 2023-07-14 16:09:45.000000 pyhandytools-0.0.5/pyhandytools.egg-info/top_level.txt
--rw-r--r--   0 jmchen     (501) staff       (20)       38 2023-07-14 16:09:45.420625 pyhandytools-0.0.5/setup.cfg
--rw-r--r--   0 jmchen     (501) staff       (20)      699 2023-07-14 16:09:35.000000 pyhandytools-0.0.5/setup.py
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:22:03.053615 pyhandytools-0.0.6/
+-rw-r--r--   0 jmchen     (501) staff       (20)    11354 2023-06-24 15:27:46.000000 pyhandytools-0.0.6/LICENSE
+-rw-r--r--   0 jmchen     (501) staff       (20)      633 2023-07-14 16:22:03.053435 pyhandytools-0.0.6/PKG-INFO
+-rw-r--r--   0 jmchen     (501) staff       (20)      202 2023-06-30 16:53:05.000000 pyhandytools-0.0.6/README.md
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:22:03.052461 pyhandytools-0.0.6/pyhandytools/
+-rw-r--r--   0 jmchen     (501) staff       (20)       48 2023-06-24 15:16:23.000000 pyhandytools-0.0.6/pyhandytools/__init__.py
+-rw-r--r--   0 jmchen     (501) staff       (20)      237 2023-07-14 16:08:13.000000 pyhandytools-0.0.6/pyhandytools/env.py
+-rw-r--r--   0 jmchen     (501) staff       (20)     1661 2023-07-14 16:08:13.000000 pyhandytools-0.0.6/pyhandytools/file.py
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-07-14 16:22:03.053241 pyhandytools-0.0.6/pyhandytools.egg-info/
+-rw-r--r--   0 jmchen     (501) staff       (20)      633 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/PKG-INFO
+-rw-r--r--   0 jmchen     (501) staff       (20)      271 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/SOURCES.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)        1 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/dependency_links.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)        7 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/requires.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)       13 2023-07-14 16:22:03.000000 pyhandytools-0.0.6/pyhandytools.egg-info/top_level.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)       38 2023-07-14 16:22:03.053668 pyhandytools-0.0.6/setup.cfg
+-rw-r--r--   0 jmchen     (501) staff       (20)      938 2023-07-14 16:21:48.000000 pyhandytools-0.0.6/setup.py
```

### Comparing `pyhandytools-0.0.5/LICENSE` & `pyhandytools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhandytools-0.0.5/pyhandytools/file.py` & `pyhandytools-0.0.6/pyhandytools/file.py`

 * *Files identical despite different names*

