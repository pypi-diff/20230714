# Comparing `tmp/supSMSGecko-0.1.0a1.tar.gz` & `tmp/supSMSGecko-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supSMSGecko-0.1.0a1.tar", last modified: Fri Jul 14 12:13:22 2023, max compression
+gzip compressed data, was "supSMSGecko-0.1.0a2.tar", last modified: Fri Jul 14 12:31:22 2023, max compression
```

## Comparing `supSMSGecko-0.1.0a1.tar` & `supSMSGecko-0.1.0a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:13:22.900052 supSMSGecko-0.1.0a1/
--rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supSMSGecko-0.1.0a1/LICENSE
--rw-rw-rw-   0        0        0       36 2023-07-14 11:51:52.000000 supSMSGecko-0.1.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0      728 2023-07-14 12:13:22.901053 supSMSGecko-0.1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supSMSGecko-0.1.0a1/README.md
--rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supSMSGecko-0.1.0a1/pyproject.toml
--rw-rw-rw-   0        0        0      678 2023-07-14 12:13:22.901053 supSMSGecko-0.1.0a1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 12:13:22.882547 supSMSGecko-0.1.0a1/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 12:13:22.885546 supSMSGecko-0.1.0a1/src/supSMSGecko/
--rw-rw-rw-   0        0        0      160 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/__init__.py
--rw-rw-rw-   0        0        0      252 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:13:22.899053 supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/
--rw-rw-rw-   0        0        0  1497824 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSE01.ld
--rw-rw-rw-   0        0        0  1490538 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSJ01.ld
--rw-rw-rw-   0        0        0  1481746 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSJ0A.ld
--rw-rw-rw-   0        0        0  1487624 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSP01.ld
--rw-rw-rw-   0        0        0     1416 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/lib.py
--rw-rw-rw-   0        0        0  5158407 2023-07-14 11:57:47.000000 supSMSGecko-0.1.0a1/src/supSMSGecko/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:13:22.895053 supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/
--rw-rw-rw-   0        0        0      728 2023-07-14 12:13:22.000000 supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-07-14 12:13:22.000000 supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:13:22.000000 supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-14 12:13:22.000000 supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 12:13:22.000000 supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.198347 supSMSGecko-0.1.0a2/
+-rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supSMSGecko-0.1.0a2/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-07-14 11:51:52.000000 supSMSGecko-0.1.0a2/MANIFEST.in
+-rw-rw-rw-   0        0        0      728 2023-07-14 12:31:22.198347 supSMSGecko-0.1.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supSMSGecko-0.1.0a2/README.md
+-rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supSMSGecko-0.1.0a2/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2023-07-14 12:31:22.201347 supSMSGecko-0.1.0a2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.179347 supSMSGecko-0.1.0a2/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.182347 supSMSGecko-0.1.0a2/src/supSMSGecko/
+-rw-rw-rw-   0        0        0      160 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-07-14 11:52:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.197347 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/
+-rw-rw-rw-   0        0        0  1497824 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSE01.ld
+-rw-rw-rw-   0        0        0  1490538 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ01.ld
+-rw-rw-rw-   0        0        0  1481746 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ0A.ld
+-rw-rw-rw-   0        0        0  1487624 2023-07-14 12:00:33.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSP01.ld
+-rw-rw-rw-   0        0        0     1471 2023-07-14 12:27:58.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/lib.py
+-rw-rw-rw-   0        0        0  5158407 2023-07-14 11:57:47.000000 supSMSGecko-0.1.0a2/src/supSMSGecko/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:31:22.192347 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/
+-rw-rw-rw-   0        0        0      728 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 12:31:22.000000 supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/top_level.txt
```

### Comparing `supSMSGecko-0.1.0a1/LICENSE` & `supSMSGecko-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a1/PKG-INFO` & `supSMSGecko-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supSMSGecko
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A helper library to write Gecko code for Super Mario Sunshine
 Home-page: https://github.com/sup39/supSMSGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supSMSGecko/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supSMSGecko-0.1.0a1/setup.cfg` & `supSMSGecko-0.1.0a2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7570 534d 5347 6563 6b6f 0d0a   = supSMSGecko..
 00000020: 7665 7273 696f 6e20 3d20 302e 312e 3061  version = 0.1.0a
-00000030: 310d 0a61 7574 686f 7220 3d20 7375 7033  1..author = sup3
+00000030: 320d 0a61 7574 686f 7220 3d20 7375 7033  2..author = sup3
 00000040: 390d 0a61 7574 686f 725f 656d 6169 6c20  9..author_email 
 00000050: 3d20 736d 7340 7375 7033 392e 6465 760d  = sms@sup39.dev.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2068 656c 7065 7220 6c69 6272 6172 7920   helper library 
 00000080: 746f 2077 7269 7465 2047 6563 6b6f 2063  to write Gecko c
 00000090: 6f64 6520 666f 7220 5375 7065 7220 4d61  ode for Super Ma
 000000a0: 7269 6f20 5375 6e73 6869 6e65 0d0a 6c6f  rio Sunshine..lo
```

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSE01.ld` & `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSE01.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSJ01.ld` & `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ01.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSJ0A.ld` & `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSJ0A.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko/ldscript/GMSP01.ld` & `supSMSGecko-0.1.0a2/src/supSMSGecko/ldscript/GMSP01.ld`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko/lib.py` & `supSMSGecko-0.1.0a2/src/supSMSGecko/lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,26 @@
   })
   main(g, version)
   return g
 
 def make_xml(
   main, versions=VERSIONS,
   info_xml='info.xml', out_xml='out.xml',
-  indent=4, tag='code',
+  indent=4, tag='code', encoding='utf8',
 ):
   if type(indent) == int: indent = ' '*indent
-  with open(out_xml, 'w') as fw:
+  with open(out_xml, 'w', encoding=encoding) as fw:
     def write_sources(indent_src):
       for ver in versions:
         print(f'{indent_src}<source version="{ver}">', file=fw)
         print(build(main, ver).dump_txt(indent_src+indent), file=fw)
         print(f'{indent_src}</source>', file=fw)
     if info_xml is not None and os.path.isfile(info_xml):
       found_tag = False
-      with open(info_xml) as f:
+      with open(info_xml, encoding=encoding) as f:
         for line in f:
           m = re.search(r'^(\s*)</(\S+)\s*>', line)
           if m is not None:
             m_tag = m.group(2)
             if m_tag == tag:
               indent_code = m.group(1)
               write_sources(indent_code+indent)
```

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko/symbols.py` & `supSMSGecko-0.1.0a2/src/supSMSGecko/symbols.py`

 * *Files identical despite different names*

### Comparing `supSMSGecko-0.1.0a1/src/supSMSGecko.egg-info/PKG-INFO` & `supSMSGecko-0.1.0a2/src/supSMSGecko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supSMSGecko
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A helper library to write Gecko code for Super Mario Sunshine
 Home-page: https://github.com/sup39/supSMSGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supSMSGecko/issues
 Classifier: Programming Language :: Python :: 3
```

