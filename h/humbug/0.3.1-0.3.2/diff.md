# Comparing `tmp/humbug-0.3.1.tar.gz` & `tmp/humbug-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humbug-0.3.1.tar", last modified: Tue Apr  4 11:38:04 2023, max compression
+gzip compressed data, was "humbug-0.3.2.tar", last modified: Thu Jul 13 22:09:02 2023, max compression
```

## Comparing `humbug-0.3.1.tar` & `humbug-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 11:38:04.093662 humbug-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     7564 2023-04-04 11:38:04.093662 humbug-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5572 2023-04-04 11:37:55.000000 humbug-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 11:38:04.089661 humbug-0.3.1/humbug/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/consent.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    19475 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/system_information.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/test_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/test_consent.py
--rw-r--r--   0 runner    (1001) docker     (122)     5903 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/test_report.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/test_system_information.py
--rw-r--r--   0 runner    (1001) docker     (122)     5857 2023-04-04 11:37:55.000000 humbug-0.3.1/humbug/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 11:38:04.093662 humbug-0.3.1/humbug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7564 2023-04-04 11:38:03.000000 humbug-0.3.1/humbug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-04 11:38:04.000000 humbug-0.3.1/humbug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 11:38:03.000000 humbug-0.3.1/humbug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-04 11:38:03.000000 humbug-0.3.1/humbug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-04 11:38:03.000000 humbug-0.3.1/humbug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 11:38:04.093662 humbug-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-04-04 11:37:55.000000 humbug-0.3.1/setup.py
+drwxrwxr-x   0 neeraj    (1000) neeraj    (1000)        0 2023-07-13 22:09:02.641084 humbug-0.3.2/
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     6161 2023-07-13 22:09:02.641084 humbug-0.3.2/PKG-INFO
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     5572 2023-07-13 21:58:14.000000 humbug-0.3.2/README.md
+drwxrwxr-x   0 neeraj    (1000) neeraj    (1000)        0 2023-07-13 22:09:02.641084 humbug-0.3.2/humbug/
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)        0 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/__init__.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     2713 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/blacklist.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     3095 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/consent.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)        0 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/py.typed
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)    19469 2023-07-13 22:07:03.000000 humbug-0.3.2/humbug/report.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)      975 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/system_information.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)      791 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/test_blacklist.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     6360 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/test_consent.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     5903 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/test_report.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)      243 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/test_system_information.py
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     5857 2023-07-13 21:58:14.000000 humbug-0.3.2/humbug/utils.py
+drwxrwxr-x   0 neeraj    (1000) neeraj    (1000)        0 2023-07-13 22:09:02.641084 humbug-0.3.2/humbug.egg-info/
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     6161 2023-07-13 22:09:02.000000 humbug-0.3.2/humbug.egg-info/PKG-INFO
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)      406 2023-07-13 22:09:02.000000 humbug-0.3.2/humbug.egg-info/SOURCES.txt
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)        1 2023-07-13 22:09:02.000000 humbug-0.3.2/humbug.egg-info/dependency_links.txt
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)      214 2023-07-13 22:09:02.000000 humbug-0.3.2/humbug.egg-info/requires.txt
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)        7 2023-07-13 22:09:02.000000 humbug-0.3.2/humbug.egg-info/top_level.txt
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)       38 2023-07-13 22:09:02.641084 humbug-0.3.2/setup.cfg
+-rw-rw-r--   0 neeraj    (1000) neeraj    (1000)     1208 2023-07-13 22:07:03.000000 humbug-0.3.2/setup.py
```

### Comparing `humbug-0.3.1/README.md` & `humbug-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/blacklist.py` & `humbug-0.3.2/humbug/blacklist.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/consent.py` & `humbug-0.3.2/humbug/consent.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/report.py` & `humbug-0.3.2/humbug/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 ```
 {error_traceback}
 ```""".format(
             user_time=int(time.time()),
             error_summary=repr(error),
             error_traceback="".join(
                 traceback.format_exception(
-                    etype=type(error),
+                    type(error),
                     value=error,
                     tb=error.__traceback__,
                 )
             ),
         )
         if tags is None:
             tags = []
```

### Comparing `humbug-0.3.1/humbug/system_information.py` & `humbug-0.3.2/humbug/system_information.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/test_blacklist.py` & `humbug-0.3.2/humbug/test_blacklist.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/test_consent.py` & `humbug-0.3.2/humbug/test_consent.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/test_report.py` & `humbug-0.3.2/humbug/test_report.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/humbug/utils.py` & `humbug-0.3.2/humbug/utils.py`

 * *Files identical despite different names*

### Comparing `humbug-0.3.1/setup.py` & `humbug-0.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = ""
 with open("README.md") as ifp:
     long_description = ifp.read()
 
 setup(
     name="humbug",
-    version="0.3.1",
+    version="0.3.2",
     packages=find_packages(),
     package_data={"humbug": ["py.typed"]},
     install_requires=["requests", "dataclasses; python_version=='3.6'"],
     extras_require={
         "dev": [
             "black",
             "mypy",
```

