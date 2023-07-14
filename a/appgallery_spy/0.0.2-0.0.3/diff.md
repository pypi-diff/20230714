# Comparing `tmp/appgallery_spy-0.0.2.tar.gz` & `tmp/appgallery_spy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appgallery_spy-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "appgallery_spy-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `appgallery_spy-0.0.2.tar` & `appgallery_spy-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       50 2023-07-13 19:36:57.498942 appgallery_spy-0.0.2/.dockerignore
--rw-r--r--   0        0        0     3082 2023-07-14 16:00:38.011538 appgallery_spy-0.0.2/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 appgallery_spy-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      925 2023-07-13 19:15:59.819245 appgallery_spy-0.0.2/Dockerfile
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appgallery_spy-0.0.2/LICENSE
--rw-r--r--   0        0        0      369 2023-07-14 17:46:54.399112 appgallery_spy-0.0.2/Makefile
--rw-r--r--   0        0        0        0 2023-07-12 00:21:08.098160 appgallery_spy-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-07-14 17:49:27.995922 appgallery_spy-0.0.2/appgallery_spy/__init__.py
--rw-r--r--   0        0        0       28 2023-07-14 17:39:28.508878 appgallery_spy-0.0.2/appgallery_spy/__main__.py
--rw-r--r--   0        0        0      911 2023-07-14 17:39:28.528870 appgallery_spy-0.0.2/appgallery_spy/api.py
--rw-r--r--   0        0        0      247 2023-07-14 17:39:27.765186 appgallery_spy-0.0.2/appgallery_spy/cli.py
--rw-r--r--   0        0        0     2563 2023-07-14 17:39:43.935138 appgallery_spy-0.0.2/appgallery_spy/crawl.py
--rw-r--r--   0        0        0      735 2023-07-14 17:39:28.532868 appgallery_spy-0.0.2/appgallery_spy/crud.py
--rw-r--r--   0        0        0      219 2023-07-14 17:39:27.721205 appgallery_spy-0.0.2/appgallery_spy/models.py
--rwxr-xr-x   0        0        0 15039112 2023-05-27 00:10:14.000000 appgallery_spy-0.0.2/chromedriver
--rw-r--r--   0        0        0      409 2023-07-13 22:04:01.035978 appgallery_spy-0.0.2/docker-compose.yml
--rw-r--r--   0        0        0     2436 2023-07-14 17:49:09.143027 appgallery_spy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      249 2023-07-14 11:24:41.897989 appgallery_spy-0.0.2/requirements.txt
--rw-r--r--   0        0        0      193 2023-07-13 19:16:53.619566 appgallery_spy-0.0.2/setup.cfg
--rw-r--r--   0        0        0      114 2023-07-13 19:16:53.159564 appgallery_spy-0.0.2/test_build.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 appgallery_spy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-13 19:36:57.498942 appgallery_spy-0.0.3/.dockerignore
+-rw-r--r--   0        0        0     3082 2023-07-14 16:00:38.011538 appgallery_spy-0.0.3/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 appgallery_spy-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      925 2023-07-13 19:15:59.819245 appgallery_spy-0.0.3/Dockerfile
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appgallery_spy-0.0.3/LICENSE
+-rw-r--r--   0        0        0      369 2023-07-14 17:46:54.399112 appgallery_spy-0.0.3/Makefile
+-rw-r--r--   0        0        0        0 2023-07-12 00:21:08.098160 appgallery_spy-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-07-14 17:53:38.062037 appgallery_spy-0.0.3/appgallery_spy/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-14 17:39:28.508878 appgallery_spy-0.0.3/appgallery_spy/__main__.py
+-rw-r--r--   0        0        0      911 2023-07-14 17:39:28.528870 appgallery_spy-0.0.3/appgallery_spy/api.py
+-rw-r--r--   0        0        0      247 2023-07-14 17:39:27.765186 appgallery_spy-0.0.3/appgallery_spy/cli.py
+-rw-r--r--   0        0        0     2563 2023-07-14 17:39:43.935138 appgallery_spy-0.0.3/appgallery_spy/crawl.py
+-rw-r--r--   0        0        0      735 2023-07-14 17:39:28.532868 appgallery_spy-0.0.3/appgallery_spy/crud.py
+-rw-r--r--   0        0        0      219 2023-07-14 17:39:27.721205 appgallery_spy-0.0.3/appgallery_spy/models.py
+-rwxr-xr-x   0        0        0 15039112 2023-05-27 00:10:14.000000 appgallery_spy-0.0.3/chromedriver
+-rw-r--r--   0        0        0      409 2023-07-13 22:04:01.035978 appgallery_spy-0.0.3/docker-compose.yml
+-rw-r--r--   0        0        0     2463 2023-07-14 17:53:26.242031 appgallery_spy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-14 17:53:26.262031 appgallery_spy-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      193 2023-07-13 19:16:53.619566 appgallery_spy-0.0.3/setup.cfg
+-rw-r--r--   0        0        0      114 2023-07-13 19:16:53.159564 appgallery_spy-0.0.3/test_build.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 appgallery_spy-0.0.3/PKG-INFO
```

### Comparing `appgallery_spy-0.0.2/.gitignore` & `appgallery_spy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/Dockerfile` & `appgallery_spy-0.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/LICENSE` & `appgallery_spy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/appgallery_spy/api.py` & `appgallery_spy-0.0.3/appgallery_spy/api.py`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/appgallery_spy/crawl.py` & `appgallery_spy-0.0.3/appgallery_spy/crawl.py`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/appgallery_spy/crud.py` & `appgallery_spy-0.0.3/appgallery_spy/crud.py`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/chromedriver` & `appgallery_spy-0.0.3/chromedriver`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.2/pyproject.toml` & `appgallery_spy-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 requires-python = ">=3.10"
 dependencies = [
     "typer >= 0.9.0",
     "fastapi >= 0.98.0",
     "uvicorn[standard] >= 0.22.0",
     "pymongo >= 4.4.1",
     "httpx >= 0.24.1",
-    "beautifulsoup4 >= 4.12.2"
+    "beautifulsoup4 >= 4.12.2",
+    "selenium >= 4.10.0",
 ]
 
 [project.scripts]
 appgallery_spy = "appgallery_spy.cli:app"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `appgallery_spy-0.0.2/PKG-INFO` & `appgallery_spy-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appgallery_spy
-Version: 0.0.2
+Version: 0.0.3
 Summary: appgallery_spy - Huauwi AppGallery Crawler
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: typer >= 0.9.0
 Requires-Dist: fastapi >= 0.98.0
 Requires-Dist: uvicorn[standard] >= 0.22.0
 Requires-Dist: pymongo >= 4.4.1
 Requires-Dist: httpx >= 0.24.1
 Requires-Dist: beautifulsoup4 >= 4.12.2
+Requires-Dist: selenium >= 4.10.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: codecov ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
```

