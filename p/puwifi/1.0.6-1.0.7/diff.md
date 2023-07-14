# Comparing `tmp/puwifi-1.0.6.tar.gz` & `tmp/puwifi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puwifi-1.0.6.tar", last modified: Thu Jul 13 15:56:37 2023, max compression
+gzip compressed data, was "puwifi-1.0.7.tar", last modified: Fri Jul 14 10:45:59 2023, max compression
```

## Comparing `puwifi-1.0.6.tar` & `puwifi-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.6/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/.github/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.6/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.6/.github/workflows/pylint.yml
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.6/.gitignore
--rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.6/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3662 2023-07-13 15:56:37.157200 puwifi-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3054 2023-07-13 15:53:55.000000 puwifi-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-13 15:56:28.000000 puwifi-1.0.6/main.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-13 15:54:51.000000 puwifi-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.6/renovate.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 15:56:37.157200 puwifi-1.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/src/puwifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3662 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9016 2023-07-13 15:45:57.000000 puwifi-1.0.6/src/puwifi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:45:59.349640 puwifi-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.7/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:45:59.339640 puwifi-1.0.7/.github/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.7/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:45:59.339640 puwifi-1.0.7/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.7/.github/workflows/pylint.yml
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.7/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.7/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-14 10:45:59.339640 puwifi-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-07-13 15:53:55.000000 puwifi-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-13 15:56:28.000000 puwifi-1.0.7/main.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-14 10:45:36.000000 puwifi-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.7/renovate.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 10:45:59.349640 puwifi-1.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:45:59.339640 puwifi-1.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:45:59.339640 puwifi-1.0.7/src/puwifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-14 10:45:59.000000 puwifi-1.0.7/src/puwifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-14 10:45:59.000000 puwifi-1.0.7/src/puwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:45:59.000000 puwifi-1.0.7/src/puwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-14 10:45:59.000000 puwifi-1.0.7/src/puwifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-14 10:45:59.000000 puwifi-1.0.7/src/puwifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 10:45:59.000000 puwifi-1.0.7/src/puwifi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9026 2023-07-14 10:43:47.000000 puwifi-1.0.7/src/puwifi.py
```

### Comparing `puwifi-1.0.6/.github/workflows/codeql-analysis.yml` & `puwifi-1.0.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.6/.github/workflows/pylint.yml` & `puwifi-1.0.7/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.6/.gitignore` & `puwifi-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.6/.pylintrc` & `puwifi-1.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.6/LICENSE` & `puwifi-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.6/PKG-INFO` & `puwifi-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.6
+Version: 1.0.7
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `puwifi-1.0.6/README.md` & `puwifi-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.6/pyproject.toml` & `puwifi-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="puwifi"
-version="1.0.6"
+version="1.0.7"
 
 authors = [
     { name="SaicharanKandukuri", email="saicharankandukuri1x1@gmail.com"}
 ]
 
 description = "⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever"
 readme = "README.md"
```

### Comparing `puwifi-1.0.6/src/puwifi.egg-info/PKG-INFO` & `puwifi-1.0.7/src/puwifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.6
+Version: 1.0.7
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `puwifi-1.0.6/src/puwifi.py` & `puwifi-1.0.7/src/puwifi.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,30 +156,30 @@
         requests.get(url, timeout=timeout)
         return True
     except (requests.ConnectionError,
             requests.Timeout):
         return False
 
 
-def keep_alive(username, password, host, port):
+def keep_alive(wu: WifiUtils,username, password, host, port):
     """keeps connection alive to wifi host"""
     while True:
 
         if connection_to("http://10.0.0.11:8090/"):
             log.info("connection to router \"available\"")
         else:
             log.critical("connection to router \"unavailable\"")
 
         if connection_to("https://google.com"):
             log.info("Connected to the internet")
         else:
             log.warning("Not connected to the internet")
             log.info("Tying to login back")
             try:
-                log.info(WifiUtils.login(username, password, host, port))
+                log.info(wu.login(username, password, host, port))
             except (requests.ConnectionError,
                     requests.Timeout):
                 log.critical(
                     "Connection error: \"UNSTABLE CONNECTION TO HOST\"")
 
         time.sleep(5)
 
@@ -239,12 +239,12 @@
                           args.password,
                           args.host, args.port,
                           ))
         sys.exit(0)
     
     if args.keep_alive:
         log.info("=> keep alive <=")
-        keep_alive(args.username,
+        keep_alive(wu,args.username,
                    args.password,
                    args.host, args.port,
                    )
```

