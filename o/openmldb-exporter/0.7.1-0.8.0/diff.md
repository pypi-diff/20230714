# Comparing `tmp/openmldb_exporter-0.7.1.tar.gz` & `tmp/openmldb_exporter-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmldb_exporter-0.7.1.tar", max compression
+gzip compressed data, was "openmldb_exporter-0.8.0.tar", max compression
```

## Comparing `openmldb_exporter-0.7.1.tar` & `openmldb_exporter-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5416 2023-02-28 02:20:42.276114 openmldb_exporter-0.7.1/README.md
--rw-r--r--   0        0        0      107 2022-05-20 04:01:39.519625 openmldb_exporter-0.7.1/openmldb_exporter/__init__.py
--rw-r--r--   0        0        0      969 2022-05-20 04:01:39.519625 openmldb_exporter-0.7.1/openmldb_exporter/collector/__init__.py
--rw-r--r--   0        0        0     6315 2023-05-19 03:47:56.696401 openmldb_exporter-0.7.1/openmldb_exporter/collector/collectors.py
--rw-r--r--   0        0        0     2857 2022-05-20 04:01:39.519625 openmldb_exporter-0.7.1/openmldb_exporter/collector/configstore.py
--rw-r--r--   0        0        0     2911 2022-05-20 04:01:39.519625 openmldb_exporter-0.7.1/openmldb_exporter/collector/metrics.py
--rw-r--r--   0        0        0     2306 2023-01-06 14:09:36.678632 openmldb_exporter-0.7.1/openmldb_exporter/exporter.py
--rw-r--r--   0        0        0     1113 2023-05-19 04:05:27.592011 openmldb_exporter-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6446 1970-01-01 00:00:00.000000 openmldb_exporter-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     5605 2023-05-21 15:05:17.714884 openmldb_exporter-0.8.0/README.md
+-rw-r--r--   0        0        0      107 2023-05-21 14:51:09.612967 openmldb_exporter-0.8.0/openmldb_exporter/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-21 14:51:09.612967 openmldb_exporter-0.8.0/openmldb_exporter/collector/__init__.py
+-rw-r--r--   0        0        0     6315 2023-05-21 14:51:09.612967 openmldb_exporter-0.8.0/openmldb_exporter/collector/collectors.py
+-rw-r--r--   0        0        0     2857 2023-05-21 14:51:09.612967 openmldb_exporter-0.8.0/openmldb_exporter/collector/configstore.py
+-rw-r--r--   0        0        0     2911 2023-05-21 14:51:09.612967 openmldb_exporter-0.8.0/openmldb_exporter/collector/metrics.py
+-rw-r--r--   0        0        0     2306 2023-05-21 14:51:09.612967 openmldb_exporter-0.8.0/openmldb_exporter/exporter.py
+-rw-r--r--   0        0        0     1113 2023-07-04 04:51:51.554086 openmldb_exporter-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 openmldb_exporter-0.8.0/PKG-INFO
```

### Comparing `openmldb_exporter-0.7.1/README.md` & `openmldb_exporter-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,7 +132,17 @@
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9520",role="tablet"} 1.6501813860467942e+09                   
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9521",role="tablet"} 1.6501813860495396e+09                   
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9522",role="tablet"} 1.650181386050323e+09                    
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9622",role="nameserver"} 1.6501813860512116e+09               
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9623",role="nameserver"} 1.650181386051238e+09                
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9624",role="nameserver"} 1.6501813860512598e+09               
    ```
+
+## Release History
+
+- 0.7.1
+    * Features
+        - Upgrade OpenMLDB SDK to v0.7
+        - Upgrade prometheus client to 0.16
+- 0.6.0
+    * Features
+        - Depends on OpenMLDB SDK v0.6
```

### Comparing `openmldb_exporter-0.7.1/openmldb_exporter/collector/__init__.py` & `openmldb_exporter-0.8.0/openmldb_exporter/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `openmldb_exporter-0.7.1/openmldb_exporter/collector/collectors.py` & `openmldb_exporter-0.8.0/openmldb_exporter/collector/collectors.py`

 * *Files identical despite different names*

### Comparing `openmldb_exporter-0.7.1/openmldb_exporter/collector/configstore.py` & `openmldb_exporter-0.8.0/openmldb_exporter/collector/configstore.py`

 * *Files identical despite different names*

### Comparing `openmldb_exporter-0.7.1/openmldb_exporter/collector/metrics.py` & `openmldb_exporter-0.8.0/openmldb_exporter/collector/metrics.py`

 * *Files identical despite different names*

### Comparing `openmldb_exporter-0.7.1/openmldb_exporter/exporter.py` & `openmldb_exporter-0.8.0/openmldb_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `openmldb_exporter-0.7.1/pyproject.toml` & `openmldb_exporter-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmldb-exporter"
-version = "0.7.1"
+version = "0.8.0"
 description = "prometheus exporter for OpenMLDB"
 authors = ["aceforeverd <teapot@aceforeverd.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://openmldb.ai"
 repository = "https://github.com/4paradigm/OpenMLDB"
 documentation = "https://openmldb.ai/docs/zh/main/maintain/monitoring.html"
@@ -17,15 +17,15 @@
 
 [tool.poetry.scripts]
 openmldb-exporter = "openmldb_exporter.exporter:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 prometheus-client = "^0.16.0"
-openmldb = "^0.7.0"
+openmldb = "^0.8.0"
 # uncomment below to use openmldb sdk built from source
 # set develop = true so changes in python will take effect immediately
 # openmldb = { path = "../python/", develop = true }
 Twisted = "^22.2.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.17.3"
```

### Comparing `openmldb_exporter-0.7.1/PKG-INFO` & `openmldb_exporter-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: openmldb-exporter
-Version: 0.7.1
+Version: 0.8.0
 Summary: prometheus exporter for OpenMLDB
 Home-page: https://openmldb.ai
 License: Apache-2.0
 Keywords: openmldb,prometheus
 Author: aceforeverd
 Author-email: teapot@aceforeverd.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: Twisted (>=22.2.0,<23.0.0)
-Requires-Dist: openmldb (>=0.7.0,<0.8.0)
+Requires-Dist: openmldb (>=0.8.0,<0.9.0)
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Project-URL: Documentation, https://openmldb.ai/docs/zh/main/maintain/monitoring.html
 Project-URL: Repository, https://github.com/4paradigm/OpenMLDB
 Description-Content-Type: text/markdown
 
 # OpenMLDB Prometheus Exporter
 
@@ -159,7 +158,17 @@
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9521",role="tablet"} 1.6501813860495396e+09                   
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9522",role="tablet"} 1.650181386050323e+09                    
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9622",role="nameserver"} 1.6501813860512116e+09               
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9623",role="nameserver"} 1.650181386051238e+09                
    openmldb_connected_seconds_created{endpoint="172.17.0.15:9624",role="nameserver"} 1.6501813860512598e+09               
    ```
 
+## Release History
+
+- 0.7.1
+    * Features
+        - Upgrade OpenMLDB SDK to v0.7
+        - Upgrade prometheus client to 0.16
+- 0.6.0
+    * Features
+        - Depends on OpenMLDB SDK v0.6
+
```

