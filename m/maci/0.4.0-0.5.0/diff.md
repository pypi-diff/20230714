# Comparing `tmp/maci-0.4.0.tar.gz` & `tmp/maci-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maci-0.4.0.tar", last modified: Wed Jul 12 05:42:09 2023, max compression
+gzip compressed data, was "maci-0.5.0.tar", last modified: Fri Jul 14 03:31:16 2023, max compression
```

## Comparing `maci-0.4.0.tar` & `maci-0.5.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-12 05:41:56.000000 maci-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-12 05:42:09.724157 maci-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-12 05:42:09.000000 maci-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/
--rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-12 05:42:09.000000 maci-0.4.0/maci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22827 2023-07-12 05:42:09.000000 maci-0.4.0/maci/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/_hash/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_hash/comparefilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_hash/createfilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_hash/createhash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/_ini/
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/inibuildauto.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/inibuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/inidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/iniload.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_json/
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsondump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsondumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsonload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsonloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_native/
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/cleanformat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6838 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/dumpraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     6134 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/dumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadattrs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loaddict.py
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadstrdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_toml/
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_xml/
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmlbuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_yaml/
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamlloadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)    73096 2023-07-12 05:42:09.000000 maci-0.4.0/maci/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7311 2023-07-12 05:42:09.000000 maci-0.4.0/maci/data.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-12 05:42:09.000000 maci-0.4.0/maci/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/ext/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/ext/defusedxml/
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-12 05:42:09.000000 maci-0.4.0/maci/ext/defusedxml/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-12 05:42:09.000000 maci-0.4.0/maci/hint.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.000000 maci-0.4.0/maci/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-12 05:42:09.728157 maci-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-12 05:41:56.000000 maci-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-14 03:31:06.000000 maci-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-14 03:31:16.296071 maci-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-14 03:31:16.000000 maci-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.288071 maci-0.5.0/maci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-14 03:31:16.000000 maci-0.5.0/maci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22867 2023-07-14 03:31:16.000000 maci-0.5.0/maci/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_hash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_hash/comparefilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_hash/createfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_hash/createhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_ini/
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/inibuildauto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/inibuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/inidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/iniload.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsondump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsondumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsonload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsonloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_native/
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/cleanformat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/dumpraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/dumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loaddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadstrdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/_toml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/_xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmlbuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamlloadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75021 2023-07-14 03:31:16.000000 maci-0.5.0/maci/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-07-14 03:31:16.000000 maci-0.5.0/maci/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-14 03:31:16.000000 maci-0.5.0/maci/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.288071 maci-0.5.0/maci/ext/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/ext/defusedxml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-14 03:31:16.000000 maci-0.5.0/maci/ext/defusedxml/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-14 03:31:16.000000 maci-0.5.0/maci/hint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-14 03:31:16.000000 maci-0.5.0/maci/hint.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.000000 maci-0.5.0/maci/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-14 03:31:16.296071 maci-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-14 03:31:06.000000 maci-0.5.0/setup.py
```

### Comparing `maci-0.4.0/PKG-INFO` & `maci-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.4.0
+Version: 0.5.0
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.4.0
+##### Latest Version: 0.5.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.4.0/README.md` & `maci-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.4.0
+##### Latest Version: 0.5.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.4.0/maci/__init__.py` & `maci-0.5.0/maci/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 maci - by aaronater10
 
 A Pythonic Configuration Language & Thin Wrapper Library
 
-Version 0.4.0
+Version 0.5.0
 
 Tutorials and docs: https://docs.macilib.org
 
 Source: https://github.com/aaronater10/maci
 """
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 #########################################################################################################
 # Imports
 
 # Exceptions
 from . import error
```

### Comparing `maci-0.4.0/maci/__init__.pyi` & `maci-0.5.0/maci/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # stub file to document public api functions, errors, object types, and doc string comments
 """
 maci - by aaronater10
 
 A Pythonic Configuration Language & Thin Wrapper Library
 
-Version 0.4.0
+Version 0.5.0
 
 Tutorials and docs: https://docs.macilib.org
 
 Source: https://github.com/aaronater10/maci
 """
 #########################################################################################################
 # Imports
@@ -20,15 +20,15 @@
 from typing import Optional as _Optional
 from typing import Set as _Set
 from types import ModuleType as _ModuleType
 from configparser import ConfigParser as _ConfigParser
 from xml.etree.ElementTree import ElementTree as _ElementTree
 from xml.etree.ElementTree import Element as _Element
 from .hint import MaciDataObj as _MaciDataObj
-from .hint import __ClassObject as _ClassObject
+from .hint import __ClassObject as _ClassObject  # type: ignore  # ignoring attr export
 
 #########################################################################################################
 # Stub data: Exceptions, Hints
 
 ### Exceptions ###
 from . import error
```

### Comparing `maci-0.4.0/maci/_hash/comparefilehash.py` & `maci-0.5.0/maci/_hash/comparefilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_hash/createfilehash.py` & `maci-0.5.0/maci/_hash/createfilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_hash/createhash.py` & `maci-0.5.0/maci/_hash/createhash.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_ini/inibuildauto.py` & `maci-0.5.0/maci/_ini/inibuildauto.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_ini/inibuildmanual.py` & `maci-0.5.0/maci/_ini/inibuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_ini/inidump.py` & `maci-0.5.0/maci/_ini/inidump.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_ini/iniload.py` & `maci-0.5.0/maci/_ini/iniload.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_json/jsondump.py` & `maci-0.5.0/maci/_json/jsondump.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_json/jsondumpstr.py` & `maci-0.5.0/maci/_json/jsondumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_json/jsonload.py` & `maci-0.5.0/maci/_json/jsonload.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_json/jsonloadstr.py` & `maci-0.5.0/maci/_json/jsonloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/build.py` & `maci-0.5.0/maci/_native/build.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/cleanformat.py` & `maci-0.5.0/maci/_native/cleanformat.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/dump.py` & `maci-0.5.0/maci/_native/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Imports
 from typing import Union as _Union
 from typing import NewType as _NewType
 from typing import Any as _Any
 from ..error import Dump
 from ..data import __dump_data
 from ..data import MaciDataObj as _MaciDataObj
-from ..hint import __ClassObject
+from ..hint import __ClassObject  # type: ignore  # ignoring attr export
 
 #########################################################################################################
 # Dump Data to File
 def dump(
     filename: str, 
     data: _Union['_MaciDataObj', dict, __ClassObject], 
     *,
```

### Comparing `maci-0.4.0/maci/_native/dumpraw.py` & `maci-0.5.0/maci/_native/dumpraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/dumpstr.py` & `maci-0.5.0/maci/_native/dumpstr.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Union as _Union
 from typing import Any as _Any
 from typing import NewType as _NewType
 from typing import Optional as _Optional
 from ..error import DumpStr
 from ..data import __dump_data
 from ..data import MaciDataObj as _MaciDataObj
-from ..hint import __ClassObject
+from ..hint import __ClassObject  # type: ignore  # ignoring attr export
 
 #########################################################################################################
 # Dump Data to String
 def dumpstr(
     data: _Union['_MaciDataObj', dict, __ClassObject], 
     *,
     indent_level: int=1,
```

### Comparing `maci-0.4.0/maci/_native/load.py` & `maci-0.5.0/maci/_native/load.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/loadattrs.py` & `maci-0.5.0/maci/_native/loadattrs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #########################################################################################################
 # Imports
 from typing import NewType as _NewType
 from typing import Union as _Union
 from ..error import LoadAttrs, Load
 from .load import load as _load
 from ..data import MaciDataObj as _MaciDataObj
-from ..hint import __ClassObject
+from ..hint import __ClassObject  # type: ignore  # ignoring attr export
 
 #########################################################################################################
 # Import Attributes from File
 def loadattrs(filename: str, class_object: __ClassObject, *, encoding: _Union[str, None]=None, attr_name_dedup: bool=False, _ignore_maci_attr_check: bool=True) -> None:
     """
     Import saved attributes from file back into a custom class. This is done in-place
```

### Comparing `maci-0.4.0/maci/_native/loaddict.py` & `maci-0.5.0/maci/_native/loaddict.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/loadraw.py` & `maci-0.5.0/maci/_native/loadraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/loadstr.py` & `maci-0.5.0/maci/_native/loadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_native/loadstrdict.py` & `maci-0.5.0/maci/_native/loadstrdict.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_toml/tomldump.py` & `maci-0.5.0/maci/_toml/tomldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_toml/tomldumpstr.py` & `maci-0.5.0/maci/_toml/tomldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_toml/tomlload.py` & `maci-0.5.0/maci/_toml/tomlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_toml/tomlloadstr.py` & `maci-0.5.0/maci/_toml/tomlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_xml/xmlbuildmanual.py` & `maci-0.5.0/maci/_xml/xmlbuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_xml/xmldump.py` & `maci-0.5.0/maci/_xml/xmldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_xml/xmldumpstr.py` & `maci-0.5.0/maci/_xml/xmldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_xml/xmlload.py` & `maci-0.5.0/maci/_xml/xmlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_xml/xmlloadstr.py` & `maci-0.5.0/maci/_xml/xmlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_yaml/yamldump.py` & `maci-0.5.0/maci/_yaml/yamldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_yaml/yamldumpstr.py` & `maci-0.5.0/maci/_yaml/yamldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_yaml/yamlload.py` & `maci-0.5.0/maci/_yaml/yamlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/_yaml/yamlloadstr.py` & `maci-0.5.0/maci/_yaml/yamlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/data.py` & `maci-0.5.0/maci/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,21 +319,21 @@
                             py_syntax_err_msg,
                             f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__file_data_line.partition(__assignment_glyph)[0].strip()} \nGot: {repr(__file_data_line)}'
                         )
                     
                     __current_assignment_glyph = __assignment_glyph.lower()
                     __var_token = __file_data_line.partition(__assignment_glyph)[0].strip()
                     __value_token = __file_data_line.partition(__assignment_glyph)[2].strip()
-                    __value_token_multi = __file_data_line.partition(__assignment_glyph)[2].split()[0].strip()
+                    __value_token_multi = __file_data_line.partition(__assignment_glyph)[2].partition(__skip_markers[2])[0].strip()
 
                     # Set Last Token with Accommodation to Multi-Line String
                     if __file_data_line.partition(__assignment_glyph)[2].strip()[-3:] in __start_markers:
                         __last_token = __file_data_line.partition(__assignment_glyph)[2].strip()[-3:]
                     else:
-                        __last_token = __file_data_line.partition(__assignment_glyph)[2].strip()[-1]
+                        __last_token = __file_data_line.partition(__assignment_glyph)[2].strip().rpartition(__skip_markers[2])[0].strip()
                     
                     try: __start_skip_token = __file_data_line.split(__assignment_glyph)[1].split()[1][0].strip()
                     except IndexError: __start_skip_token = ''  # nosec: B105  # not password
                 
                 # Collect End Token if in Build
                 if __is_building_data_sw:
                     try:
@@ -472,14 +472,21 @@
                             setattr(self, __var_token, datetime_format)
                         else:
                             raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
 
             else: raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num}')
     
 
+
+    def __getattr__(self, _name: str) -> _Any:
+        if _name in self.__dict__:  # pragma: no cover  # not evaluating but is used/operating
+            return self.__dict__[_name]
+        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{_name}'")
+
+
     def __setattr__(self, _name: str, _new_value: _Any) -> None:
         # Check if Attr Already Exists, if so, Collect Original Value
         if hasattr(self, _name):
             _orig_value = self.__dict__.get(_name)
             
         # Release Attribute Reference if Name is Re-Assigned
         if hasattr(self, _name):
@@ -949,14 +956,42 @@
         attr_parent = 'some value'
 
         attr_child == attr_parent
 
         Child map will be -> {'attr_child': 'attr_parent'}
         """
         return _deepcopy(self.__assigned_src_reference_attr_map)
+    
+
+    @_rename_exc_name_to_user_object_name
+    def get_attrs(self) -> _Dict[str, _Any]:
+        """
+        Returns a dict copy of the MaciDataObj's current attribute names and values
+        """
+        skip_name_keys = ('_MaciDataObjConstructor', '__maci_obj_format_id')
+        return {name:value for name,value in self.__dict__.items() if not name.startswith(skip_name_keys)}
+    
+
+    @_rename_exc_name_to_user_object_name
+    def load_attrs(self, data: _Dict[str, _Any]) -> None:
+        """
+        Loads data from a dict into the MaciDataObj in-place
+        
+        Creates new attribute names with their values retained based on the top level key names of the dict
+
+        Note: If the key name is not a valid pythonic name convention, it will be skipped
+        """
+        err_msg_type_data = "Only dict is allowed for 'data'"
+        if not isinstance(data, dict): raise GeneralError(err_msg_type_data, f'\nGot: {repr(data)}')
+
+        for attr,value in data.items():
+            # Validate is String and Identifier for valid Attr Names, otherwise skip
+            if not isinstance(attr, str): continue
+            if not attr.isidentifier(): continue            
+            setattr(self, attr, value)
 
 
 #########################################################################################################
 # Main MaciDataObj Reference
 
 # Meta for structure references
 class __MaciDataObj(type):
@@ -1009,32 +1044,38 @@
                 _assignment_locked_atrribs_err_msg=_assignment_locked_atrribs_err_msg,
                 _assignment_hard_locked_atrribs_err_msg=_assignment_hard_locked_atrribs_err_msg,
                 _is_str_parse_request=_is_str_parse_request,
                 _str_data=_str_data,
                 _is_build_request=_is_build_request,
                 _ignore_internal_maci_attr_check=_ignore_internal_maci_attr_check,
             )
-    
+
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, MaciDataObj):
             return NotImplemented
         else:
             # Compare str repr of maci objects, which contain actual attrs & values in strings
             return str(self) == str(other)
 
     def __bool__(self) -> bool:
         skip_name_keys = ('_MaciDataObjConstructor', '__maci_obj_format_id')
-        if [attr for attr in vars(self) if not attr.startswith(skip_name_keys)]:
+        if [attr for attr in self.__dict__ if not attr.startswith(skip_name_keys)]:
             return True
         return False
 
     def __repr__(self) -> str:
         skip_name_keys = ('_MaciDataObjConstructor', '__maci_obj_format_id')
-        build_repr = ', '.join(f"{name}={value!r}" for name,value in vars(self).items() if not name.startswith(skip_name_keys))
+        build_repr = ', '.join(f"{name}={value!r}" for name,value in self.__dict__.items() if not name.startswith(skip_name_keys))
         return f"{type(self).__name__}({build_repr})"
+    
+    def __dir__(self) -> _List[str]:
+        skip_name_keys = ('_MaciDataObjConstructor', '__maci_obj_format_id')
+        default_attrs = list(name for name in dir(MaciDataObj) if not name.startswith(skip_name_keys))
+        user_attrs = list(name for name in self.__dict__ if not name.startswith(skip_name_keys))
+        return default_attrs + user_attrs
 
 
 #########################################################################################################
 # Main Dump Function
 
 # Hinting reference name for "ClassObject" to denote a ClassObject can be used to dump data
 ClassObject = _TypeVar('ClassObject')
```

### Comparing `maci-0.4.0/maci/data.pyi` & `maci-0.5.0/maci/data.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -161,27 +161,50 @@
         """
         Returns a new dict of the current child reference maps
 
         [Example: Map Structure]
 
         {'attr_child1': 'attr_parent1', 'attr_child2': 'attr_parent1'}
         """
+    
+    def get_attrs(self) -> _Dict[str, _Any]:
+        """
+        Returns a dict copy of the MaciDataObj's current attribute names and values
+        """
+
+    def load_attrs(self, data: _Dict[str, _Any]) -> None:
+        """
+        Loads data from a dict into the MaciDataObj in-place
+        
+        Creates new attribute names with their values retained based on the top level key names of the dict
+
+        Note: If the key name is not a valid pythonic name convention, it will be skipped
+        """
+    
+    def __getattr__(self, _name: str) -> _Any:
+        ...
+
+    def __setattr__(self, _name: str, _new_value: _Any) -> None:
+        ...
+    
+    def __dir__(self) -> _List[str]:
+        ...
 
 
 #########################################################################################################
 # Stub data: Functions
 
 # Hinting reference name for "ClassObject" to denote a ClassObject can be used to dump data
 ClassObject = _TypeVar('ClassObject')
 
 def __dump_data(
     *,
     _is_string_request: bool=False,
     filename: str,
-    data: _Any, # objects allowed: MaciDataObj, dict, ClassObject - ignoring type checker
+    data: _Union[MaciDataObj, dict, ClassObject],
     append: bool=False,
     indent_level: int=1,
     indentation_on: bool=True,
     multi_line_str: bool=False,
     encoding: _Union[str, None]=None,
     class_attrs: bool=False,
     private_attrs: bool=False,
```

### Comparing `maci-0.4.0/maci/error.py` & `maci-0.5.0/maci/error.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/ext/defusedxml/LICENSE.txt` & `maci-0.5.0/maci/ext/defusedxml/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci/hint.py` & `maci-0.5.0/maci/hint.py`

 * *Files identical despite different names*

### Comparing `maci-0.4.0/maci.egg-info/PKG-INFO` & `maci-0.5.0/maci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.4.0
+Version: 0.5.0
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.4.0
+##### Latest Version: 0.5.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.4.0/maci.egg-info/SOURCES.txt` & `maci-0.5.0/maci.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ./README.md
 maci/__init__.py
 maci/__init__.pyi
 maci/data.py
 maci/data.pyi
 maci/error.py
 maci/hint.py
+maci/hint.pyi
 maci/py.typed
 maci.egg-info/PKG-INFO
 maci.egg-info/SOURCES.txt
 maci.egg-info/dependency_links.txt
 maci.egg-info/requires.txt
 maci.egg-info/top_level.txt
 maci/_hash/comparefilehash.py
```

### Comparing `maci-0.4.0/setup.cfg` & `maci-0.5.0/setup.cfg`

 * *Files identical despite different names*

