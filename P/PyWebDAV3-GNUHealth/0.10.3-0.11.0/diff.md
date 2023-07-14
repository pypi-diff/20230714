# Comparing `tmp/PyWebDAV3-GNUHealth-0.10.3.tar.gz` & `tmp/PyWebDAV3-GNUHealth-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyWebDAV3-GNUHealth-0.10.3.tar", last modified: Tue Nov  6 13:41:50 2018, max compression
+gzip compressed data, was "PyWebDAV3-GNUHealth-0.11.0.tar", last modified: Fri Jul 14 16:18:24 2023, max compression
```

## Comparing `PyWebDAV3-GNUHealth-0.10.3.tar` & `PyWebDAV3-GNUHealth-0.11.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/
--rw-r--r--   0 lfm       (1000) users      (100)       94 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/MANIFEST.in
--rw-r--r--   0 lfm       (1000) users      (100)    11234 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/PKG-INFO
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/
--rw-r--r--   0 lfm       (1000) users      (100)    11234 2018-11-06 13:41:49.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/PKG-INFO
--rw-r--r--   0 lfm       (1000) users      (100)     1045 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt
--rw-r--r--   0 lfm       (1000) users      (100)        1 2018-11-06 13:41:49.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/dependency_links.txt
--rw-r--r--   0 lfm       (1000) users      (100)       58 2018-11-06 13:41:49.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/entry_points.txt
--rw-r--r--   0 lfm       (1000) users      (100)        1 2018-11-06 13:41:49.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/not-zip-safe
--rw-r--r--   0 lfm       (1000) users      (100)        9 2018-11-06 13:41:49.000000 PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/top_level.txt
--rw-r--r--   0 lfm       (1000) users      (100)      367 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/README
--rw-r--r--   0 lfm       (1000) users      (100)        7 2018-11-06 13:27:16.000000 PyWebDAV3-GNUHealth-0.10.3/VERSION
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/doc/
--rw-r--r--   0 lfm       (1000) users      (100)     2824 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/doc/ARCHITECTURE
--rw-r--r--   0 lfm       (1000) users      (100)     7733 2018-11-06 13:34:52.000000 PyWebDAV3-GNUHealth-0.10.3/doc/Changes
--rw-r--r--   0 lfm       (1000) users      (100)      394 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/doc/INSTALL
--rw-r--r--   0 lfm       (1000) users      (100)    35147 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/doc/LICENSE
--rw-r--r--   0 lfm       (1000) users      (100)      684 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/doc/TODO
--rw-r--r--   0 lfm       (1000) users      (100)     4150 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/doc/interface_class
--rw-r--r--   0 lfm       (1000) users      (100)     1234 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/doc/walker
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/
--rw-r--r--   0 lfm       (1000) users      (100)        0 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/__init__.py
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/
--rw-r--r--   0 lfm       (1000) users      (100)     3370 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/AuthServer.py
--rw-r--r--   0 lfm       (1000) users      (100)     1566 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/INI_Parse.py
--rw-r--r--   0 lfm       (1000) users      (100)    24707 2018-09-01 14:43:29.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/WebDAVServer.py
--rw-r--r--   0 lfm       (1000) users      (100)      375 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/__init__.py
--rw-r--r--   0 lfm       (1000) users      (100)      648 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/constants.py
--rw-r--r--   0 lfm       (1000) users      (100)     5289 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/davcmd.py
--rw-r--r--   0 lfm       (1000) users      (100)     3204 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/davcopy.py
--rw-r--r--   0 lfm       (1000) users      (100)     2260 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/davmove.py
--rw-r--r--   0 lfm       (1000) users      (100)     2180 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/dbconn.py
--rw-r--r--   0 lfm       (1000) users      (100)      612 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/delete.py
--rw-r--r--   0 lfm       (1000) users      (100)     1489 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/errors.py
--rw-r--r--   0 lfm       (1000) users      (100)     8554 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/iface.py
--rw-r--r--   0 lfm       (1000) users      (100)     8182 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/locks.py
--rw-r--r--   0 lfm       (1000) users      (100)    11892 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/propfind.py
--rw-r--r--   0 lfm       (1000) users      (100)     4387 2018-01-04 13:21:46.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/report.py
--rw-r--r--   0 lfm       (1000) users      (100)      554 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/status.py
--rw-r--r--   0 lfm       (1000) users      (100)     6898 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/utils.py
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/
--rw-r--r--   0 lfm       (1000) users      (100)        1 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/__init__.py
--rw-r--r--   0 lfm       (1000) users      (100)     1053 2018-01-04 13:21:46.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/config.ini
--rw-r--r--   0 lfm       (1000) users      (100)     5429 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/daemonize.py
--rw-r--r--   0 lfm       (1000) users      (100)     1844 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/fileauth.py
--rw-r--r--   0 lfm       (1000) users      (100)    11696 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/fshandler.py
--rw-r--r--   0 lfm       (1000) users      (100)     1970 2018-01-04 13:21:46.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/mysqlauth.py
--rw-r--r--   0 lfm       (1000) users      (100)    12937 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/server.py
--rw-r--r--   0 lfm       (1000) users      (100)       59 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/setup.cfg
--rw-r--r--   0 lfm       (1000) users      (100)     1896 2018-01-04 13:21:45.000000 PyWebDAV3-GNUHealth-0.10.3/setup.py
-drwxr-xr-x   0 lfm       (1000) users      (100)        0 2018-11-06 13:41:50.000000 PyWebDAV3-GNUHealth-0.10.3/test/
--rw-r--r--   0 lfm       (1000) users      (100)     3884 2018-01-04 13:21:46.000000 PyWebDAV3-GNUHealth-0.10.3/test/test_litmus.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322672 PyWebDAV3-GNUHealth-0.11.0/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)       94 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/MANIFEST.in
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1236 2023-07-14 16:18:24.322752 PyWebDAV3-GNUHealth-0.11.0/PKG-INFO
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.320032 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1236 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/PKG-INFO
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1041 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/dependency_links.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)       57 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/entry_points.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/not-zip-safe
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        9 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/top_level.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      367 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/README.rst
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.320695 PyWebDAV3-GNUHealth-0.11.0/doc/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     2824 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/ARCHITECTURE
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     7836 2023-07-14 15:40:07.000000 PyWebDAV3-GNUHealth-0.11.0/doc/Changes
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      394 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/INSTALL
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    35147 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/LICENSE
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      684 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/TODO
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     4150 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/interface_class
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1234 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/walker
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.320769 PyWebDAV3-GNUHealth-0.11.0/pywebdav/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        0 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/__init__.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322006 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     3370 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/AuthServer.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1566 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/INI_Parse.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    24513 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/WebDAVServer.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      375 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/__init__.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      648 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/constants.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     5289 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcmd.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     3204 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcopy.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     2260 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davmove.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     2180 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/dbconn.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      612 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/delete.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1489 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/errors.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     8554 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/iface.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     8182 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/locks.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    11779 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/propfind.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     4387 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/report.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      554 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/status.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     6838 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/utils.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322522 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/__init__.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1053 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/config.ini
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     5429 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/daemonize.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1844 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fileauth.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    11645 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fshandler.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1970 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/mysqlauth.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    12937 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/server.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)       59 2023-07-14 16:18:24.322994 PyWebDAV3-GNUHealth-0.11.0/setup.cfg
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1520 2023-07-14 16:15:07.000000 PyWebDAV3-GNUHealth-0.11.0/setup.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322602 PyWebDAV3-GNUHealth-0.11.0/test/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     3884 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/test/test_litmus.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt` & `PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 MANIFEST.in
-README
-VERSION
+README.rst
 setup.cfg
 setup.py
 PyWebDAV3_GNUHealth.egg-info/PKG-INFO
 PyWebDAV3_GNUHealth.egg-info/SOURCES.txt
 PyWebDAV3_GNUHealth.egg-info/dependency_links.txt
 PyWebDAV3_GNUHealth.egg-info/entry_points.txt
 PyWebDAV3_GNUHealth.egg-info/not-zip-safe
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/doc/ARCHITECTURE` & `PyWebDAV3-GNUHealth-0.11.0/doc/ARCHITECTURE`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/doc/Changes` & `PyWebDAV3-GNUHealth-0.11.0/doc/Changes`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.11.0 (July 2023)
+-----------------
+Fix encoding issues in Thunderbird
+Enforce str - utf8, not Bytes
+
 0.10.2 (Sept 1, 2018)
 ---------------------
 Check for binary type before encoding
 
 0.10.2 (July 15 2017)
 ---------------------
 Fix WebDAVServer data string conversion to make it compatible with older
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/doc/LICENSE` & `PyWebDAV3-GNUHealth-0.11.0/doc/LICENSE`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/doc/TODO` & `PyWebDAV3-GNUHealth-0.11.0/doc/TODO`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/doc/interface_class` & `PyWebDAV3-GNUHealth-0.11.0/doc/interface_class`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/doc/walker` & `PyWebDAV3-GNUHealth-0.11.0/doc/walker`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/AuthServer.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/AuthServer.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/INI_Parse.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/INI_Parse.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/WebDAVServer.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/WebDAVServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,34 +95,31 @@
             self.send_header('Content-Length', len(DATA))
             self.send_header('Content-Type', ctype)
         else:
             self.send_header('Content-Length', 0)
 
         self.end_headers()
         if DATA:
-            if (isinstance(DATA, bytes)):
-                self.wfile.write(DATA)
-            else:
-                self.wfile.write(DATA.encode('utf-8'))
-            
             if isinstance(DATA, str):
                 log.debug("Don't use iterator")
                 self.wfile.write(DATA.encode('utf-8'))
-            else:
+            elif (isinstance(DATA, bytes)):
 
                 if self._config.DAV.getboolean('http_response_use_iterator'):
                     # Use iterator to reduce using memory
                     log.debug("Use iterator")
                     for buf in DATA:
                         self.wfile.write(buf)
                         self.wfile.flush()
                 else:
                     # Don't use iterator, it's a compatibility option
                     log.debug("Don't use iterator")
                     self.wfile.write(DATA)
+            else:
+                self.send_header('Content-Length', 0)
             
         return None
 
     def send_body_chunks_if_http11(self, DATA, code, msg=None, desc=None,
                                    ctype='text/xml; encoding="utf-8"',
                                    headers={}):
 
@@ -160,15 +157,14 @@
                         output.write(buf)
                 output.close()
                 buffer.seek(0)
                 DATA = buffer.getvalue()
                 self.send_header('Content-Encoding', 'gzip')
 
             self.send_header('Content-Length', len(DATA))
-            self.send_header('Content-Type', ctype)
 
         else:
             self.send_header('Content-Length', 0)
 
         self.end_headers()
 
         if DATA:
@@ -222,15 +218,15 @@
         self.end_headers()
 
     def _HEAD_GET(self, with_body=False):
         """ Returns headers and body for given resource """
 
         dc = self.IFACE_CLASS
         uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        uri = urllib.parse.unquote(uri).encode()
+        uri = urllib.parse.unquote(uri)
 
         headers = {}
 
         # get the last modified date (RFC 1123!)
         try:
             headers['Last-Modified'] = dc.get_prop(
                 uri, "DAV:", "getlastmodified")
@@ -326,15 +322,15 @@
         # iff there is no body then this is an ALLPROP request
         body = None
         if 'Content-Length' in self.headers:
             l = self.headers['Content-Length']
             body = self.rfile.read(int(l))
 
         uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        uri = urllib.parse.unquote(uri).encode()
+        uri = urllib.parse.unquote(uri)
 
         try:
             pf = PROPFIND(uri, dc, self.headers.get('Depth', 'infinity'), body)
         except ExpatError:
             # parse error
             return self.send_status(400)
 
@@ -372,15 +368,15 @@
         # iff there is no body then this is an ALLPROP request
         body = None
         if 'Content-Length' in self.headers:
             l = self.headers['Content-Length']
             body = self.rfile.read(int(l))
 
         uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        uri = urllib.parse.unquote(uri).encode()
+        uri = urllib.parse.unquote(uri)
 
         rp = REPORT(uri, dc, self.headers.get('Depth', '0'), body)
 
         try:
             DATA = rp.createResponse() + b'\n'
         except DAV_Error as error:
             (ec, dd) = error.args
@@ -399,15 +395,15 @@
             body = self.rfile.read(int(l))
 
         if body:
             return self.send_status(415)
 
         dc = self.IFACE_CLASS
         uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        uri = urllib.parse.unquote(uri).encode()
+        uri = urllib.parse.unquote(uri)
 
         try:
             dc.mkcol(uri)
             self.send_status(201)
             self.log_request(201)
         except DAV_Error as error:
             (ec, dd) = error.args
@@ -415,18 +411,18 @@
             return self.send_status(ec)
 
     def do_DELETE(self):
         """ delete an resource """
 
         dc = self.IFACE_CLASS
         uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        uri = urllib.parse.unquote(uri).encode()
+        uri = urllib.parse.unquote(uri)
 
         # hastags not allowed
-        if uri.find(b'#') >= 0:
+        if uri.find('#') >= 0:
             return self.send_status(404)
 
         # locked resources are not allowed to delete
         if self._l_isLocked(uri):
             return self.send_body(None, 423, 'Locked', 'Locked')
 
         # Handle If-Match
@@ -486,15 +482,15 @@
                 self.send_status(res)
         except DAV_NotFound:
             self.send_body(None, 404, 'Not Found', 'Not Found')
 
     def do_PUT(self):
         dc = self.IFACE_CLASS
         uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        uri = urllib.parse.unquote(uri).encode()
+        uri = urllib.parse.unquote(uri)
 
         log.debug("do_PUT: uri = %s" % uri)
         log.debug('do_PUT: headers = %s' % self.headers)
         # Handle If-Match
         if 'If-Match' in self.headers:
             log.debug("do_PUT: If-Match %s" % self.headers['If-Match'])
             test = False
@@ -673,19 +669,19 @@
 
     def copymove(self, CLASS):
         """ common method for copying or moving objects """
         dc = self.IFACE_CLASS
 
         # get the source URI
         source_uri = urllib.parse.urljoin(self.get_baseuri(dc), self.path)
-        source_uri = urllib.parse.unquote(source_uri).encode()
+        source_uri = urllib.parse.unquote(source_uri)
 
         # get the destination URI
         dest_uri = self.headers['Destination']
-        dest_uri = urllib.parse.unquote(dest_uri).encode()
+        dest_uri = urllib.parse.unquote(dest_uri)
 
         # check locks on source and dest
         if self._l_isLocked(source_uri) or self._l_isLocked(dest_uri):
             return self.send_body(None, 423, 'Locked', 'Locked')
 
         # Overwrite?
         overwrite = 1
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/constants.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/constants.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/davcmd.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcmd.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/davcopy.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcopy.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/davmove.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davmove.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/dbconn.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/dbconn.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/delete.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/delete.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/errors.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/errors.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/iface.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/iface.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/locks.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/locks.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/propfind.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/propfind.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(self, uri, dataclass, depth, body):
         self.request_type = None
         self.nsmap = {}
         self.proplist = {}
         self.default_ns = None
         self._dataclass = dataclass
         self._depth = str(depth)
-        self._uri = uri.rstrip(b'/')
+        self._uri = uri.rstrip('/')
         self._has_body = None   # did we parse a body?
 
         if dataclass.verbose:
             log.info('PROPFIND: Depth is %s, URI is %s' % (depth, uri))
 
         if body:
             self.request_type, self.proplist, self.namespaces = \
@@ -241,18 +241,15 @@
                 re.setAttribute("xmlns:ns" + str(nsnum), nsname)
             nsnum += 1
 
         if self._dataclass.baseurl:
             uri = self._dataclass.baseurl + '/' + '/'.join(uri.split('/')[3:])
 
         # write href information
-        if not isinstance(uri, str):
-            uparts = urllib.parse.urlparse(uri.decode())
-        else:
-            uparts = urllib.parse.urlparse(uri)
+        uparts = urllib.parse.urlparse(uri)
 
         fileloc = uparts[2]
         href = doc.createElement("D:href")
 
         huri = doc.createTextNode(uparts[0] + '://' +
                                   '/'.join(uparts[1:2]) +
                                   urllib.parse.quote(fileloc))
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/report.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/report.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/status.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/status.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/lib/utils.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         return 1
     else:
         return None
 
 def quote_uri(uri):
     """ quote an URL but not the protocol part """
     up=urllib.parse.urlparse(uri)
-    # np=urllib.parse.quote(up[2]).encode('utf-8')
     np=urllib.parse.quote(up[2])
     return urllib.parse.urlunparse((up[0],up[1],np,up[3],up[4],up[5]))
 
 def get_uriparentpath(uri):
     """ extract the uri path and remove the last element """
     up=urllib.parse.urlparse(uri)
     return "/".join(up[2].split("/")[:-1])
@@ -100,15 +99,15 @@
     up=urllib.parse.urlparse(uri)
     res = up[2]
     res = res.split("/")[-1]
     return res
 
 def get_parenturi(uri):
     """ return the parent of the given resource"""
-    up=urllib.parse.urlparse(uri).decode()
+    up=urllib.parse.urlparse(uri)
 
     np='/'.join(up[2].split("/")[:-1])
     return urllib.parse.urlunparse((up[0],up[1],np,up[3],up[4],up[5]))
 
 ### XML utilities
 
 def make_xmlresponse(result):
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/config.ini` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/config.ini`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/daemonize.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/daemonize.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/fileauth.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fileauth.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/fshandler.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fshandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,28 +81,28 @@
     def setBaseURI(self, uri):
         """ Sets the base uri """
 
         self.baseuri = uri
 
     def uri2local(self,uri):
         """ map uri in baseuri and local part """
-        uparts=urllib.parse.urlparse(uri.decode())
+        uparts=urllib.parse.urlparse(uri)
         fileloc=uparts[2][1:]
         filename=os.path.join(self.directory, fileloc)
         filename=os.path.normpath(filename)
         return filename
 
     def local2uri(self,filename):
         """ map local filename to self.baseuri """
 
         pnum=len(self.directory.replace("\\","/").split("/"))
         parts=filename.replace("\\","/").split("/")[pnum:]
         sparts="/"+"/".join(parts)
         uri=urllib.parse.urljoin(self.baseuri,sparts)
-        return uri.encode() if isinstance(uri, str) else uri
+        return uri
 
 
     def get_childs(self, uri, filter=None):
         """ return the child objects as self.baseuris for the given URI """
 
         fileloc=self.uri2local(uri)
         filelist=[]
```

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/mysqlauth.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/mysqlauth.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/pywebdav/server/server.py` & `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/server.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.10.3/test/test_litmus.py` & `PyWebDAV3-GNUHealth-0.11.0/test/test_litmus.py`

 * *Files identical despite different names*

