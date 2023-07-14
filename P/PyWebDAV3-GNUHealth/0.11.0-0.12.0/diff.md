# Comparing `tmp/PyWebDAV3-GNUHealth-0.11.0.tar.gz` & `tmp/PyWebDAV3-GNUHealth-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyWebDAV3-GNUHealth-0.11.0.tar", last modified: Fri Jul 14 16:18:24 2023, max compression
+gzip compressed data, was "PyWebDAV3-GNUHealth-0.12.0.tar", last modified: Fri Jul 14 16:45:44 2023, max compression
```

## Comparing `PyWebDAV3-GNUHealth-0.11.0.tar` & `PyWebDAV3-GNUHealth-0.12.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322672 PyWebDAV3-GNUHealth-0.11.0/
--rw-r--r--   0 lfm       (1001) lfm       (1001)       94 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/MANIFEST.in
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1236 2023-07-14 16:18:24.322752 PyWebDAV3-GNUHealth-0.11.0/PKG-INFO
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.320032 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1236 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/PKG-INFO
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1041 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt
--rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/dependency_links.txt
--rw-r--r--   0 lfm       (1001) lfm       (1001)       57 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/entry_points.txt
--rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/not-zip-safe
--rw-r--r--   0 lfm       (1001) lfm       (1001)        9 2023-07-14 16:18:24.000000 PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/top_level.txt
--rw-r--r--   0 lfm       (1001) lfm       (1001)      367 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/README.rst
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.320695 PyWebDAV3-GNUHealth-0.11.0/doc/
--rw-r--r--   0 lfm       (1001) lfm       (1001)     2824 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/ARCHITECTURE
--rw-r--r--   0 lfm       (1001) lfm       (1001)     7836 2023-07-14 15:40:07.000000 PyWebDAV3-GNUHealth-0.11.0/doc/Changes
--rw-r--r--   0 lfm       (1001) lfm       (1001)      394 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/INSTALL
--rw-r--r--   0 lfm       (1001) lfm       (1001)    35147 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/LICENSE
--rw-r--r--   0 lfm       (1001) lfm       (1001)      684 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/TODO
--rw-r--r--   0 lfm       (1001) lfm       (1001)     4150 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/interface_class
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1234 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/doc/walker
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.320769 PyWebDAV3-GNUHealth-0.11.0/pywebdav/
--rw-r--r--   0 lfm       (1001) lfm       (1001)        0 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/__init__.py
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322006 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/
--rw-r--r--   0 lfm       (1001) lfm       (1001)     3370 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/AuthServer.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1566 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/INI_Parse.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)    24513 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/WebDAVServer.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)      375 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/__init__.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)      648 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/constants.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     5289 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcmd.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     3204 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcopy.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     2260 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davmove.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     2180 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/dbconn.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)      612 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/delete.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1489 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/errors.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     8554 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/iface.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     8182 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/locks.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)    11779 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/propfind.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     4387 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/report.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)      554 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/status.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     6838 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/utils.py
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322522 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/
--rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/__init__.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1053 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/config.ini
--rw-r--r--   0 lfm       (1001) lfm       (1001)     5429 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/daemonize.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1844 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fileauth.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)    11645 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fshandler.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1970 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/mysqlauth.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)    12937 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/server.py
--rw-r--r--   0 lfm       (1001) lfm       (1001)       59 2023-07-14 16:18:24.322994 PyWebDAV3-GNUHealth-0.11.0/setup.cfg
--rw-r--r--   0 lfm       (1001) lfm       (1001)     1520 2023-07-14 16:15:07.000000 PyWebDAV3-GNUHealth-0.11.0/setup.py
-drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:18:24.322602 PyWebDAV3-GNUHealth-0.11.0/test/
--rw-r--r--   0 lfm       (1001) lfm       (1001)     3884 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.11.0/test/test_litmus.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.369590 PyWebDAV3-GNUHealth-0.12.0/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)       99 2023-07-14 16:34:13.000000 PyWebDAV3-GNUHealth-0.12.0/MANIFEST.in
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1236 2023-07-14 16:45:44.369441 PyWebDAV3-GNUHealth-0.12.0/PKG-INFO
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.366621 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1236 2023-07-14 16:45:44.000000 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/PKG-INFO
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1039 2023-07-14 16:45:44.000000 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 16:45:44.000000 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/dependency_links.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)       57 2023-07-14 16:45:44.000000 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/entry_points.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 16:45:44.000000 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/not-zip-safe
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        9 2023-07-14 16:45:44.000000 PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/top_level.txt
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      367 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/README.rst
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.367310 PyWebDAV3-GNUHealth-0.12.0/doc/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     2824 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/doc/ARCHITECTURE
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     7924 2023-07-14 16:36:29.000000 PyWebDAV3-GNUHealth-0.12.0/doc/Changes
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      394 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/doc/INSTALL
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    35147 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/doc/LICENSE
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      684 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/doc/TODO
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     4150 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/doc/interface_class
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1234 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/doc/walker
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.367415 PyWebDAV3-GNUHealth-0.12.0/pywebdav/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        0 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/__init__.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.368696 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     3370 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/AuthServer.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1566 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/INI_Parse.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    24513 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/WebDAVServer.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      375 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/__init__.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      648 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/constants.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     5289 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/davcmd.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     3204 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/davcopy.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     2260 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/davmove.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     2180 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/dbconn.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      612 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/delete.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1489 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/errors.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     8554 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/iface.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     8182 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/locks.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    11779 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/propfind.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     4387 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/report.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)      554 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/status.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     6838 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/utils.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.369222 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        1 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/__init__.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1053 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/config.ini
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     5429 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/daemonize.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1844 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/fileauth.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    11645 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/fshandler.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1970 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/mysqlauth.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)    12937 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/server.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)       38 2023-07-14 16:45:44.369629 PyWebDAV3-GNUHealth-0.12.0/setup.cfg
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     1500 2023-07-14 16:25:09.000000 PyWebDAV3-GNUHealth-0.12.0/setup.py
+drwxr-xr-x   0 lfm       (1001) lfm       (1001)        0 2023-07-14 16:45:44.369301 PyWebDAV3-GNUHealth-0.12.0/test/
+-rw-r--r--   0 lfm       (1001) lfm       (1001)     3884 2023-07-14 15:28:43.000000 PyWebDAV3-GNUHealth-0.12.0/test/test_litmus.py
+-rw-r--r--   0 lfm       (1001) lfm       (1001)        7 2023-07-14 16:35:11.000000 PyWebDAV3-GNUHealth-0.12.0/version
```

### Comparing `PyWebDAV3-GNUHealth-0.11.0/PKG-INFO` & `PyWebDAV3-GNUHealth-0.12.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWebDAV3-GNUHealth
-Version: 0.11.0
+Version: 0.12.0
 Summary: WebDAV library for Python3 - GNU Health port
 Home-page: https://www.gnuhealth.org
 Download-URL: https://ftp.gnu.org/gnu/health/
 Author: GNU Solidario
 Author-email: health@gnusolidario.org
 Maintainer: GNU Health team
 Maintainer-email: info@gnuhealth.org
```

### Comparing `PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/PKG-INFO` & `PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWebDAV3-GNUHealth
-Version: 0.11.0
+Version: 0.12.0
 Summary: WebDAV library for Python3 - GNU Health port
 Home-page: https://www.gnuhealth.org
 Download-URL: https://ftp.gnu.org/gnu/health/
 Author: GNU Solidario
 Author-email: health@gnusolidario.org
 Maintainer: GNU Health team
 Maintainer-email: info@gnuhealth.org
```

### Comparing `PyWebDAV3-GNUHealth-0.11.0/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt` & `PyWebDAV3-GNUHealth-0.12.0/PyWebDAV3_GNUHealth.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 README.rst
-setup.cfg
 setup.py
+version
 PyWebDAV3_GNUHealth.egg-info/PKG-INFO
 PyWebDAV3_GNUHealth.egg-info/SOURCES.txt
 PyWebDAV3_GNUHealth.egg-info/dependency_links.txt
 PyWebDAV3_GNUHealth.egg-info/entry_points.txt
 PyWebDAV3_GNUHealth.egg-info/not-zip-safe
 PyWebDAV3_GNUHealth.egg-info/top_level.txt
 doc/ARCHITECTURE
```

### Comparing `PyWebDAV3-GNUHealth-0.11.0/doc/ARCHITECTURE` & `PyWebDAV3-GNUHealth-0.12.0/doc/ARCHITECTURE`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/doc/Changes` & `PyWebDAV3-GNUHealth-0.12.0/doc/Changes`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.11.1 (July 14, 2023)
+-----------------
+Include version and README.rst in MANIFEST.in
+
 0.11.0 (July 2023)
 -----------------
 Fix encoding issues in Thunderbird
 Enforce str - utf8, not Bytes
 
 0.10.2 (Sept 1, 2018)
 ---------------------
```

### Comparing `PyWebDAV3-GNUHealth-0.11.0/doc/LICENSE` & `PyWebDAV3-GNUHealth-0.12.0/doc/LICENSE`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/doc/TODO` & `PyWebDAV3-GNUHealth-0.12.0/doc/TODO`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/doc/interface_class` & `PyWebDAV3-GNUHealth-0.12.0/doc/interface_class`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/doc/walker` & `PyWebDAV3-GNUHealth-0.12.0/doc/walker`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/AuthServer.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/AuthServer.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/INI_Parse.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/INI_Parse.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/WebDAVServer.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/WebDAVServer.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/constants.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/constants.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcmd.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/davcmd.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davcopy.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/davcopy.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/davmove.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/davmove.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/dbconn.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/dbconn.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/delete.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/delete.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/errors.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/errors.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/iface.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/iface.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/locks.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/locks.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/propfind.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/propfind.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/report.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/report.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/status.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/status.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/lib/utils.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/lib/utils.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/config.ini` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/config.ini`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/daemonize.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/daemonize.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fileauth.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/fileauth.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/fshandler.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/fshandler.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/mysqlauth.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/mysqlauth.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/pywebdav/server/server.py` & `PyWebDAV3-GNUHealth-0.12.0/pywebdav/server/server.py`

 * *Files identical despite different names*

### Comparing `PyWebDAV3-GNUHealth-0.11.0/setup.py` & `PyWebDAV3-GNUHealth-0.12.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
-from io import open
 
 long_desc = open("README.rst").read()
 version = open("version").read().strip()
 
 setup(name='PyWebDAV3-GNUHealth',
       version=version,
       description='WebDAV library for Python3 - GNU Health port',
```

### Comparing `PyWebDAV3-GNUHealth-0.11.0/test/test_litmus.py` & `PyWebDAV3-GNUHealth-0.12.0/test/test_litmus.py`

 * *Files identical despite different names*

