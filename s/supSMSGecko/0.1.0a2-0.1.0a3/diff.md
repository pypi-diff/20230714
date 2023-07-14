# Comparing `tmp/supSMSGecko-0.1.0a2.tar.gz` & `tmp/supSMSGecko-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supSMSGecko-0.1.0a2.tar", last modified: Fri Jul 14 12:31:22 2023, max compression
+gzip compressed data, was "supSMSGecko-0.1.0a3.tar", last modified: Fri Jul 14 12:50:39 2023, max compression
```

## Comparing `supSMSGecko-0.1.0a2.tar` & `supSMSGecko-0.1.0a3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.198347 supSMSGecko-0.1.0a2/
--rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supSMSGecko-0.1.0a2/LICENSE
--rw-rw-rw-   0        0        0       36 2023-07-14 11:51:52.000000 supSMSGecko-0.1.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0      728 2023-07-14 12:31:22.198347 supSMSGecko-0.1.0a2/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supSMSGecko-0.1.0a2/README.md
--rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supSMSGecko-0.1.0a2/pyproject.toml
--rw-rw-rw-   0        0        0      678 2023-07-14 12:31:22.201347 supSMSGecko-0.1.0a2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.179347 supSMSGecko-0.1.0a2/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.182347 supSMSGecko-0.1.0a2/src/supSMSGecko/
--rw-rw-rw-   0        0        0      160 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/__init__.py
--rw-rw-rw-   0        0        0      252 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.197347 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/
--rw-rw-rw-   0        0        0  1497824 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSE01.ld
--rw-rw-rw-   0        0        0  1490538 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ01.ld
--rw-rw-rw-   0        0        0  1481746 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ0A.ld
--rw-rw-rw-   0        0        0  1487624 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSP01.ld
--rw-rw-rw-   0        0        0     1471 2023-07-14 12:27:58.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/lib.py
--rw-rw-rw-   0        0        0  5158407 2023-07-14 11:57:47.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.192347 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/
--rw-rw-rw-   0        0        0      728 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:39.922654 supSMSGecko-0.1.0a3/
+-rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supSMSGecko-0.1.0a3/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-07-14 11:51:52.000000 supSMSGecko-0.1.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0      728 2023-07-14 12:50:39.922654 supSMSGecko-0.1.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supSMSGecko-0.1.0a3/README.md
+-rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supSMSGecko-0.1.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2023-07-14 12:50:39.923652 supSMSGecko-0.1.0a3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:39.903652 supSMSGecko-0.1.0a3/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:39.907652 supSMSGecko-0.1.0a3/src/supSMSGecko/
+-rw-rw-rw-   0        0        0      160 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:39.921652 supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/
+-rw-rw-rw-   0        0        0  1497824 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSE01.ld
+-rw-rw-rw-   0        0        0  1490538 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSJ01.ld
+-rw-rw-rw-   0        0        0  1481746 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSJ0A.ld
+-rw-rw-rw-   0        0        0  1487624 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSP01.ld
+-rw-rw-rw-   0        0        0     1473 2023-07-14 12:49:13.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/lib.py
+-rw-rw-rw-   0        0        0  5158407 2023-07-14 11:57:47.000000 supSMSGecko-0.1.0a3/src/supSMSGecko/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:39.917652 supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/
+-rw-rw-rw-   0        0        0      728 2023-07-14 12:50:39.000000 supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-07-14 12:50:39.000000 supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:50:39.000000 supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-14 12:50:39.000000 supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 12:50:39.000000 supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/top_level.txt
```

### Comparing `supSMSGecko-0.1.0a2/LICENSE` & `supSMSGecko-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a2/PKG-INFO` & `supSMSGecko-0.1.0a3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supSMSGecko
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A helper library to write Gecko code for Super Mario Sunshine
 Home-page: https://github.com/sup39/supSMSGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supSMSGecko/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supSMSGecko-0.1.0a2/setup.cfg` & `supSMSGecko-0.1.0a3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7570 534d 5347 6563 6b6f 0d0a   = supSMSGecko..
 00000020: 7665 7273 696f 6e20 3d20 302e 312e 3061  version = 0.1.0a
-00000030: 320d 0a61 7574 686f 7220 3d20 7375 7033  2..author = sup3
+00000030: 330d 0a61 7574 686f 7220 3d20 7375 7033  3..author = sup3
 00000040: 390d 0a61 7574 686f 725f 656d 6169 6c20  9..author_email 
 00000050: 3d20 736d 7340 7375 7033 392e 6465 760d  = sms@sup39.dev.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2068 656c 7065 7220 6c69 6272 6172 7920   helper library 
 00000080: 746f 2077 7269 7465 2047 6563 6b6f 2063  to write Gecko c
 00000090: 6f64 6520 666f 7220 5375 7065 7220 4d61  ode for Super Ma
 000000a0: 7269 6f20 5375 6e73 6869 6e65 0d0a 6c6f  rio Sunshine..lo
```

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSE01.ld` & `supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSE01.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ01.ld` & `supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSJ01.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ0A.ld` & `supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSJ0A.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSP01.ld` & `supSMSGecko-0.1.0a3/src/supSMSGecko/ldscript/GMSP01.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko/lib.py` & `supSMSGecko-0.1.0a3/src/supSMSGecko/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'ld_flags': ['-T', f'{__dirname__}/ldscript/{version}.ld'],
   })
   main(g, version)
   return g
 
 def make_xml(
   main, versions=VERSIONS,
-  info_xml='info.xml', out_xml='out.xml',
+  info_xml='info.xml', out_xml='@code.xml',
   indent=4, tag='code', encoding='utf8',
 ):
   if type(indent) == int: indent = ' '*indent
   with open(out_xml, 'w', encoding=encoding) as fw:
     def write_sources(indent_src):
       for ver in versions:
         print(f'{indent_src}<source version="{ver}">', file=fw)
```

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko/symbols.py` & `supSMSGecko-0.1.0a3/src/supSMSGecko/symbols.py`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/PKG-INFO` & `supSMSGecko-0.1.0a3/src/supSMSGecko.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supSMSGecko
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A helper library to write Gecko code for Super Mario Sunshine
 Home-page: https://github.com/sup39/supSMSGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supSMSGecko/issues
 Classifier: Programming Language :: Python :: 3
```

