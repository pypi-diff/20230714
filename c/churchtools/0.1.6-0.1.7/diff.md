# Comparing `tmp/churchtools-0.1.6.tar.gz` & `tmp/churchtools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "churchtools-0.1.6.tar", last modified: Fri Jul 14 08:38:39 2023, max compression
+gzip compressed data, was "churchtools-0.1.7.tar", last modified: Fri Jul 14 08:42:29 2023, max compression
```

## Comparing `churchtools-0.1.6.tar` & `churchtools-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-14 08:38:39.449741 churchtools-0.1.6/
--rw-r--r--   0 philipp    (501) staff       (20)    35149 2023-02-27 13:02:42.000000 churchtools-0.1.6/LICENSE
--rw-r--r--   0 philipp    (501) staff       (20)     2064 2023-07-14 08:38:39.449588 churchtools-0.1.6/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)     1591 2023-07-14 08:29:40.000000 churchtools-0.1.6/README.md
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-14 08:38:39.448701 churchtools-0.1.6/churchtools/
--rw-r--r--   0 philipp    (501) staff       (20)     8197 2023-05-19 09:13:41.000000 churchtools-0.1.6/churchtools/__init__.py
--rw-r--r--   0 philipp    (501) staff       (20)     2061 2023-04-28 16:35:53.000000 churchtools-0.1.6/churchtools/calendars.py
--rw-r--r--   0 philipp    (501) staff       (20)    11211 2023-07-14 08:18:22.000000 churchtools-0.1.6/churchtools/ct_types.py
--rw-r--r--   0 philipp    (501) staff       (20)      629 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/departments.py
--rw-r--r--   0 philipp    (501) staff       (20)     3241 2023-06-30 06:43:47.000000 churchtools-0.1.6/churchtools/events.py
--rw-r--r--   0 philipp    (501) staff       (20)     2475 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/general.py
--rw-r--r--   0 philipp    (501) staff       (20)    11764 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/persons.py
--rw-r--r--   0 philipp    (501) staff       (20)     1031 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/services.py
--rw-r--r--   0 philipp    (501) staff       (20)     2365 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/songs.py
--rw-r--r--   0 philipp    (501) staff       (20)     1202 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/status.py
--rw-r--r--   0 philipp    (501) staff       (20)     3607 2023-02-27 13:02:42.000000 churchtools-0.1.6/churchtools/wiki.py
-drwxr-xr-x   0 philipp    (501) staff       (20)        0 2023-07-14 08:38:39.449385 churchtools-0.1.6/churchtools.egg-info/
--rw-r--r--   0 philipp    (501) staff       (20)     2064 2023-07-14 08:38:39.000000 churchtools-0.1.6/churchtools.egg-info/PKG-INFO
--rw-r--r--   0 philipp    (501) staff       (20)      455 2023-07-14 08:38:39.000000 churchtools-0.1.6/churchtools.egg-info/SOURCES.txt
--rw-r--r--   0 philipp    (501) staff       (20)        1 2023-07-14 08:38:39.000000 churchtools-0.1.6/churchtools.egg-info/dependency_links.txt
--rw-r--r--   0 philipp    (501) staff       (20)       18 2023-07-14 08:38:39.000000 churchtools-0.1.6/churchtools.egg-info/requires.txt
--rw-r--r--   0 philipp    (501) staff       (20)       12 2023-07-14 08:38:39.000000 churchtools-0.1.6/churchtools.egg-info/top_level.txt
--rw-r--r--   0 philipp    (501) staff       (20)       38 2023-07-14 08:38:39.449780 churchtools-0.1.6/setup.cfg
--rw-r--r--   0 philipp    (501) staff       (20)      990 2023-07-14 08:38:09.000000 churchtools-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:42:29.161047 churchtools-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 08:42:20.000000 churchtools-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 08:42:29.161047 churchtools-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 08:42:20.000000 churchtools-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:42:29.157047 churchtools-0.1.7/churchtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/calendars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/ct_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/persons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 08:42:20.000000 churchtools-0.1.7/churchtools/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:42:29.157047 churchtools-0.1.7/churchtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 08:42:29.000000 churchtools-0.1.7/churchtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:42:29.161047 churchtools-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 08:42:20.000000 churchtools-0.1.7/setup.py
```

### Comparing `churchtools-0.1.6/LICENSE` & `churchtools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/PKG-INFO` & `churchtools-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: churchtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for the ChurchTools API
 Home-page: https://git.sr.ht/~pglaum/pychurchtools
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api churchtools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `churchtools-0.1.6/README.md` & `churchtools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/__init__.py` & `churchtools-0.1.7/churchtools/__init__.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/calendars.py` & `churchtools-0.1.7/churchtools/calendars.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/ct_types.py` & `churchtools-0.1.7/churchtools/ct_types.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/departments.py` & `churchtools-0.1.7/churchtools/departments.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/events.py` & `churchtools-0.1.7/churchtools/events.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/general.py` & `churchtools-0.1.7/churchtools/general.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/persons.py` & `churchtools-0.1.7/churchtools/persons.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/services.py` & `churchtools-0.1.7/churchtools/services.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/songs.py` & `churchtools-0.1.7/churchtools/songs.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/status.py` & `churchtools-0.1.7/churchtools/status.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools/wiki.py` & `churchtools-0.1.7/churchtools/wiki.py`

 * *Files identical despite different names*

### Comparing `churchtools-0.1.6/churchtools.egg-info/PKG-INFO` & `churchtools-0.1.7/churchtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: churchtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for the ChurchTools API
 Home-page: https://git.sr.ht/~pglaum/pychurchtools
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api churchtools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `churchtools-0.1.6/setup.py` & `churchtools-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="churchtools",
-    version="0.1.6",
+    version="0.1.7",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A library for the ChurchTools API"),
     license="GPLv3",
     keywords="api churchtools",
     url="https://git.sr.ht/~pglaum/pychurchtools",
     packages=["churchtools"],
```

