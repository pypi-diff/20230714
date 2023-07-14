# Comparing `tmp/reliableGPT-0.2.992.tar.gz` & `tmp/reliableGPT-0.2.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.992.tar", last modified: Fri Jul 14 01:13:48 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.993.tar", last modified: Fri Jul 14 01:17:31 2023, max compression
```

## Comparing `reliableGPT-0.2.992.tar` & `reliableGPT-0.2.993.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:13:48.256941 reliableGPT-0.2.992/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.992/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:13:48.256773 reliableGPT-0.2.992/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.992/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.992/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:13:48.255280 reliableGPT-0.2.992/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:13:48.000000 reliableGPT-0.2.992/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 01:13:48.000000 reliableGPT-0.2.992/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 01:13:48.000000 reliableGPT-0.2.992/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       63 2023-07-14 01:13:48.000000 reliableGPT-0.2.992/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 01:13:48.000000 reliableGPT-0.2.992/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:13:48.256482 reliableGPT-0.2.992/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.992/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    22294 2023-07-14 01:13:13.000000 reliableGPT-0.2.992/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.992/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.992/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:04:10.000000 reliableGPT-0.2.992/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 01:13:48.256980 reliableGPT-0.2.992/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      418 2023-07-14 01:13:38.000000 reliableGPT-0.2.992/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:17:31.014086 reliableGPT-0.2.993/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.993/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:17:31.013939 reliableGPT-0.2.993/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.993/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.993/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:17:31.012811 reliableGPT-0.2.993/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:17:30.000000 reliableGPT-0.2.993/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 01:17:30.000000 reliableGPT-0.2.993/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 01:17:30.000000 reliableGPT-0.2.993/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       63 2023-07-14 01:17:30.000000 reliableGPT-0.2.993/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 01:17:30.000000 reliableGPT-0.2.993/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:17:31.013789 reliableGPT-0.2.993/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.993/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    22294 2023-07-14 01:13:13.000000 reliableGPT-0.2.993/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.993/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.993/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:17:16.000000 reliableGPT-0.2.993/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 01:17:31.014125 reliableGPT-0.2.993/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      418 2023-07-14 01:17:22.000000 reliableGPT-0.2.993/setup.py
```

### Comparing `reliableGPT-0.2.992/LICENSE` & `reliableGPT-0.2.993/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.992/README.md` & `reliableGPT-0.2.993/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.992/reliablegpt/Alerting.py` & `reliableGPT-0.2.993/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.992/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.993/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.992/reliablegpt/Model.py` & `reliableGPT-0.2.993/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.992/reliablegpt/main.py` & `reliableGPT-0.2.993/reliablegpt/main.py`

 * *Files identical despite different names*

