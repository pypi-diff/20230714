# Comparing `tmp/p3do-0.7.1.tar.gz` & `tmp/p3do-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3do-0.7.1.tar", max compression
+gzip compressed data, was "p3do-0.7.2.tar", max compression
```

## Comparing `p3do-0.7.1.tar` & `p3do-0.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-15 11:36:21.727748 p3do-0.7.1/LICENSE
--rw-r--r--   0        0        0    15444 2023-06-15 11:36:21.727748 p3do-0.7.1/README.md
--rw-r--r--   0        0        0       22 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/__init__.py
--rw-r--r--   0        0        0    13964 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/cli.py
--rw-r--r--   0        0        0      274 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/github.py
--rw-r--r--   0        0        0     1832 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/jenkins.py
--rw-r--r--   0        0        0     1161 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/keycloak.py
--rw-r--r--   0        0        0     4626 2023-06-15 11:36:21.727748 p3do-0.7.1/p3do/poolparty.py
--rw-r--r--   0        0        0      936 2023-06-15 11:36:21.727748 p3do-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    16424 1970-01-01 00:00:00.000000 p3do-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-14 12:34:35.426638 p3do-0.7.2/LICENSE
+-rw-r--r--   0        0        0    15444 2023-07-14 12:34:35.426638 p3do-0.7.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/__init__.py
+-rw-r--r--   0        0        0    13964 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/cli.py
+-rw-r--r--   0        0        0      274 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/github.py
+-rw-r--r--   0        0        0     1798 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/jenkins.py
+-rw-r--r--   0        0        0     1161 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/keycloak.py
+-rw-r--r--   0        0        0     4626 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/poolparty.py
+-rw-r--r--   0        0        0      938 2023-07-14 12:34:35.426638 p3do-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    16424 1970-01-01 00:00:00.000000 p3do-0.7.2/PKG-INFO
```

### Comparing `p3do-0.7.1/LICENSE` & `p3do-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `p3do-0.7.1/README.md` & `p3do-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `p3do-0.7.1/p3do/cli.py` & `p3do-0.7.2/p3do/cli.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.1/p3do/jenkins.py` & `p3do-0.7.2/p3do/jenkins.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     # This will start the job and will return a QueueItem object which
     # can be used to get build results
     jk_job = server[job]
     logger.debug("Got job {}", jk_job)
     qi = jk_job.invoke(build_params=params)
     logger.debug("Got job invocation {}", qi)
 
-    breakpoint()
     logger.info("Block until building")
     qi.block_until_building()
     logger.info("Started build {}", qi.get_build())
     return qi.get_build().get_build_url()
 
 
 @logger.catch
@@ -46,12 +45,11 @@
     # This will start the job and will return a QueueItem object which
     # can be used to get build results
     jk_job = server[job]
     logger.debug("Got job {}", jk_job)
     qi = jk_job.invoke(build_params=params)
     logger.debug("Got job invocation {}", qi)
 
-    breakpoint()
     logger.info("Block until building")
     qi.block_until_building()
     logger.info("Started build {}", qi.get_build())
     return qi.get_build().get_build_url()
```

### Comparing `p3do-0.7.1/p3do/keycloak.py` & `p3do-0.7.2/p3do/keycloak.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.1/p3do/poolparty.py` & `p3do-0.7.2/p3do/poolparty.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.1/pyproject.toml` & `p3do-0.7.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "p3do"
-version = "0.7.1"
+version = "0.7.2"
 description = "CLI utilities for p3d"
 authors = ["Armin Friedl <armin.friedl@semantic-web.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -19,15 +19,15 @@
 jenkinsapi = "^0.3.11"
 loguru = "^0.6.0"
 rich = "^12.4.4"
 Flask = "^2.1.3"
 pygithub = "^1.58.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^7.0.2"
 black = "^22.3.0"
 pyflakes = "^2.4.0"
 isort = "^5.10.1"
 
 [tool.poetry.scripts]
 p3do = 'p3do.cli:cli'
```

### Comparing `p3do-0.7.1/PKG-INFO` & `p3do-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3do
-Version: 0.7.1
+Version: 0.7.2
 Summary: CLI utilities for p3d
 License: MIT
 Author: Armin Friedl
 Author-email: armin.friedl@semantic-web.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

