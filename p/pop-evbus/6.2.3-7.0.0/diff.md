# Comparing `tmp/pop-evbus-6.2.3.tar.gz` & `tmp/pop-evbus-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-evbus-6.2.3.tar", last modified: Tue Mar 14 19:45:47 2023, max compression
+gzip compressed data, was "pop-evbus-7.0.0.tar", last modified: Fri Jul 14 20:33:08 2023, max compression
```

## Comparing `pop-evbus-6.2.3.tar` & `pop-evbus-7.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3283 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2409 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/
--rw-r--r--   0 root         (0) root         (0)      455 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/evbus/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/evbus/acct.py
--rw-r--r--   0 root         (0) root         (0)     4452 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/evbus/broker.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/evbus/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/ingress/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/ingress/contracts/
--rw-r--r--   0 root         (0) root         (0)       54 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/ingress/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/ingress/internal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/log/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/log/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/match/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/evbus/match/contracts/
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/match/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/match/glob.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/match/init.py
--rw-r--r--   0 root         (0) root         (0)      105 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/evbus/match/regex.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-14 19:45:47.000000 pop-evbus-6.2.3/evbus/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/pop_evbus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3283 2023-03-14 19:45:47.000000 pop-evbus-6.2.3/pop_evbus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-03-14 19:45:47.000000 pop-evbus-6.2.3/pop_evbus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 19:45:47.000000 pop-evbus-6.2.3/pop_evbus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-14 19:45:47.000000 pop-evbus-6.2.3/pop_evbus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-14 19:45:47.000000 pop-evbus-6.2.3/pop_evbus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      255 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-14 19:45:47.733827 pop-evbus-6.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2748 2023-03-14 19:45:34.000000 pop-evbus-6.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/evbus/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/evbus/acct.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/evbus/broker.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/evbus/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/ingress/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/ingress/contracts/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/ingress/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/ingress/internal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/log/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/log/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/match/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/evbus/match/contracts/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/match/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/match/glob.py
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/match/init.py
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/evbus/match/regex.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-14 20:33:08.000000 pop-evbus-7.0.0/evbus/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/pop_evbus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-07-14 20:33:08.000000 pop-evbus-7.0.0/pop_evbus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-14 20:33:08.000000 pop-evbus-7.0.0/pop_evbus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 20:33:08.000000 pop-evbus-7.0.0/pop_evbus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-14 20:33:08.000000 pop-evbus-7.0.0/pop_evbus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-14 20:33:08.000000 pop-evbus-7.0.0/pop_evbus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 20:33:08.882340 pop-evbus-7.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-07-14 20:32:54.000000 pop-evbus-7.0.0/setup.py
```

### Comparing `pop-evbus-6.2.3/LICENSE` & `pop-evbus-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/PKG-INFO` & `pop-evbus-7.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pop-evbus
-Version: 6.2.3
+Version: 7.0.0
 Summary: Event propagation to configured ingress plugins
 Home-page: https://gitlab.com/saltstack/pop/evbus
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =====
 EVBUS
 =====
```

### Comparing `pop-evbus-6.2.3/README.rst` & `pop-evbus-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/evbus/evbus/acct.py` & `pop-evbus-7.0.0/evbus/evbus/acct.py`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/evbus/evbus/broker.py` & `pop-evbus-7.0.0/evbus/evbus/broker.py`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/evbus/evbus/init.py` & `pop-evbus-7.0.0/evbus/evbus/init.py`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/evbus/ingress/internal.py` & `pop-evbus-7.0.0/evbus/ingress/internal.py`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/evbus/log/queue.py` & `pop-evbus-7.0.0/evbus/log/queue.py`

 * *Files identical despite different names*

### Comparing `pop-evbus-6.2.3/pop_evbus.egg-info/PKG-INFO` & `pop-evbus-7.0.0/pop_evbus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pop-evbus
-Version: 6.2.3
+Version: 7.0.0
 Summary: Event propagation to configured ingress plugins
 Home-page: https://gitlab.com/saltstack/pop/evbus
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =====
 EVBUS
 =====
```

### Comparing `pop-evbus-6.2.3/setup.py` & `pop-evbus-7.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,24 +70,24 @@
     url="https://gitlab.com/saltstack/pop/evbus",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 )
```

