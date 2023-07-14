# Comparing `tmp/port4me-0.5.1.post9006.tar.gz` & `tmp/port4me-0.6.0.tar.gz`

## Comparing `port4me-0.5.1.post9006.tar` & `port4me-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/Makefile
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/NEWS.md
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/port4me/__init__.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/port4me/__main__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/tests/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/tests/port4me.bats
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/tests/test_port4me.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/tests/test_uint_hash.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/LICENSE
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/pyproject.toml
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 port4me-0.5.1.post9006/PKG-INFO
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 port4me-0.6.0/Makefile
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 port4me-0.6.0/NEWS.md
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 port4me-0.6.0/port4me/__init__.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 port4me-0.6.0/port4me/__main__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 port4me-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 port4me-0.6.0/tests/port4me.bats
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 port4me-0.6.0/tests/test_port4me.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 port4me-0.6.0/tests/test_uint_hash.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 port4me-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 port4me-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 port4me-0.6.0/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 port4me-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 port4me-0.6.0/PKG-INFO
```

### Comparing `port4me-0.5.1.post9006/Makefile` & `port4me-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/port4me/__init__.py` & `port4me-0.6.0/port4me/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from itertools import islice
 import socket
 from getpass import getuser
 from os import getenv
 
 
-__version__ = "0.5.1-9006"
+__version__ = "0.6.0"
 __all__ = ["port4me", "port4me_gen"]
 
 
 # Source: https://chromium.googlesource.com/chromium/src.git/+/refs/heads/master/net/base/port_util.cc
 # Last updated: 2022-10-24
 unsafe_ports_chrome = getenv("PORT4ME_EXCLUDE_UNSAFE_CHROME", "1,7,9,11,13,15,17,19,20,21,22,23,25,37,42,43,53,69,77,79,87,95,101,102,103,104,109,110,111,113,115,117,119,123,135,137,139,143,161,179,389,427,465,512,513,514,515,526,530,531,532,540,548,554,556,563,587,601,636,989,990,993,995,1719,1720,1723,2049,3659,4045,5060,5061,6000,6566,6665,6666,6667,6668,6669,6697,10080")
```

### Comparing `port4me-0.5.1.post9006/port4me/__main__.py` & `port4me-0.6.0/port4me/__main__.py`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/tests/port4me.bats` & `port4me-0.6.0/tests/port4me.bats`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/tests/test_port4me.py` & `port4me-0.6.0/tests/test_port4me.py`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/LICENSE` & `port4me-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/README.md` & `port4me-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/pyproject.toml` & `port4me-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9006/PKG-INFO` & `port4me-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port4me
-Version: 0.5.1.post9006
+Version: 0.6.0
 Summary: The 'port4me' tool: (1) finds a free TCP port in [1024,65535] that the user can open, (2) is designed to work in multi-user environments, (3), gives different users, different ports, (4) gives the user the same port over time with high probability, (5) gives different ports for different software tools, and (6) requires no configuration.
 Project-URL: Homepage, https://github.com/HenrikBengtsson/port4me
 Project-URL: Bug Tracker, https://github.com/HenrikBengtsson/port4me/issues
 Author-email: "Finn Reichertz, Henrik Bengtsson" <henrikb@braju.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

