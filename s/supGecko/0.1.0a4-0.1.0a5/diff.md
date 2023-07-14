# Comparing `tmp/supGecko-0.1.0a4.tar.gz` & `tmp/supGecko-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supGecko-0.1.0a4.tar", last modified: Fri Jul 14 11:43:34 2023, max compression
+gzip compressed data, was "supGecko-0.1.0a5.tar", last modified: Fri Jul 14 14:00:15 2023, max compression
```

## Comparing `supGecko-0.1.0a4.tar` & `supGecko-0.1.0a5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.402558 supGecko-0.1.0a4/
--rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supGecko-0.1.0a4/LICENSE
--rw-rw-rw-   0        0        0      694 2023-07-14 11:43:34.402558 supGecko-0.1.0a4/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supGecko-0.1.0a4/README.md
--rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supGecko-0.1.0a4/pyproject.toml
--rw-rw-rw-   0        0        0      623 2023-07-14 11:43:34.404562 supGecko-0.1.0a4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.379558 supGecko-0.1.0a4/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.395558 supGecko-0.1.0a4/src/supGecko/
--rw-rw-rw-   0        0        0       88 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/__init__.py
--rw-rw-rw-   0        0        0     2840 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/asm.py
--rw-rw-rw-   0        0        0      359 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/consts.py
--rw-rw-rw-   0        0        0     8591 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/gecko.py
--rw-rw-rw-   0        0        0     1381 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.401561 supGecko-0.1.0a4/src/supGecko.egg-info/
--rw-rw-rw-   0        0        0      694 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 14:00:15.922490 supGecko-0.1.0a5/
+-rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supGecko-0.1.0a5/LICENSE
+-rw-rw-rw-   0        0        0      694 2023-07-14 14:00:15.922490 supGecko-0.1.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supGecko-0.1.0a5/README.md
+-rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supGecko-0.1.0a5/pyproject.toml
+-rw-rw-rw-   0        0        0      633 2023-07-14 14:00:15.926490 supGecko-0.1.0a5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 14:00:15.911984 supGecko-0.1.0a5/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 14:00:15.915984 supGecko-0.1.0a5/src/supGecko/
+-rw-rw-rw-   0        0        0       88 2023-07-14 11:34:52.000000 supGecko-0.1.0a5/src/supGecko/__init__.py
+-rw-rw-rw-   0        0        0     3245 2023-07-14 13:57:01.000000 supGecko-0.1.0a5/src/supGecko/asm.py
+-rw-rw-rw-   0        0        0      418 2023-07-14 11:46:09.000000 supGecko-0.1.0a5/src/supGecko/consts.py
+-rw-rw-rw-   0        0        0     8591 2023-07-14 11:34:52.000000 supGecko-0.1.0a5/src/supGecko/gecko.py
+-rw-rw-rw-   0        0        0     1440 2023-07-14 11:46:13.000000 supGecko-0.1.0a5/src/supGecko/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:00:15.922490 supGecko-0.1.0a5/src/supGecko.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-07-14 14:00:15.000000 supGecko-0.1.0a5/src/supGecko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-14 14:00:15.000000 supGecko-0.1.0a5/src/supGecko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:00:15.000000 supGecko-0.1.0a5/src/supGecko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 14:00:15.000000 supGecko-0.1.0a5/src/supGecko.egg-info/top_level.txt
```

### Comparing `supGecko-0.1.0a4/LICENSE` & `supGecko-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `supGecko-0.1.0a4/PKG-INFO` & `supGecko-0.1.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supGecko
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A helper library to write Gecko code
 Home-page: https://github.com/sup39/supGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supGecko/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supGecko-0.1.0a4/setup.cfg` & `supGecko-0.1.0a5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7570 4765 636b 6f0d 0a76 6572   = supGecko..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 6134 0d0a  sion = 0.1.0a4..
+00000020: 7369 6f6e 203d 2030 2e31 2e30 6135 0d0a  sion = 0.1.0a5..
 00000030: 6175 7468 6f72 203d 2073 7570 3339 0d0a  author = sup39..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
 00000050: 6d73 4073 7570 3339 2e64 6576 0d0a 6465  ms@sup39.dev..de
 00000060: 7363 7269 7074 696f 6e20 3d20 4120 6865  scription = A he
 00000070: 6c70 6572 206c 6962 7261 7279 2074 6f20  lper library to 
 00000080: 7772 6974 6520 4765 636b 6f20 636f 6465  write Gecko code
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -23,17 +23,18 @@
 00000160: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
 00000170: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
 00000180: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 00000190: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
 000001a0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
 000001b0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
 000001c0: 656e 7365 0d0a 0d0a 5b6f 7074 696f 6e73  ense....[options
-000001d0: 5d0d 0a69 6e63 6c75 6465 5f70 6163 6b61  ]..include_packa
-000001e0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-000001f0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-00000200: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000210: 7320 3d20 3e3d 332e 380d 0a0d 0a5b 6f70  s = >=3.8....[op
-00000220: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000230: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000240: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-00000250: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000260: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000001d0: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
+000001e0: 6e64 5f6e 616d 6573 7061 6365 3a0d 0a69  nd_namespace:..i
+000001f0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000200: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
+00000210: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000220: 332e 380d 0a0d 0a5b 6f70 7469 6f6e 732e  3.8....[options.
+00000230: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000240: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000250: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000260: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000270: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `supGecko-0.1.0a4/src/supGecko/asm.py` & `supGecko-0.1.0a5/src/supGecko/asm.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 
 import shutil
 from distutils import spawn
 import tempfile
 import os
 import subprocess
 
-def system(argv, *args, **kwargs):
-  r = subprocess.run(argv, *args, capture_output=True, text=True, **kwargs)
+def system(argv, *, catch=None, **kwargs):
+  r = subprocess.run(argv, capture_output=True, text=True, **kwargs)
   if r.returncode:
-    raise Exception(f'Fail to run {argv[0]} (code={r.returncode}): {r.stderr}')
+    if catch is not None:
+      # catch(r) returns the alternate stdout for handled errors
+      o = catch(r)
+      # if catch(r) returns None, the error is unexpected and should be raised
+      if o is not None: return o
+    raise Exception(f'Fail to run {argv} (code={r.returncode}): {r.stderr}')
   return r.stdout
 
 def write_extra_input(x, file):
   if type(x) == str:
     print(x, file=file)
   else:
     for line in x:
@@ -79,18 +84,19 @@
       '-T', distLD,
       *extra_ld_flags,
       distOBJ,
     ])
 
     # gecko symbols
     symbols = {}
+    errmsg_nosymbol = "section '.text' mentioned in a -j option, but not found in any input file"
     lines = system([
       'powerpc-eabi-objdump',
       '-tj.text', distLOBJ,
-    ]).split('\n')
+    ], catch=lambda r: '' if r.returncode==1 and errmsg_nosymbol in r.stderr else None).split('\n')
     for line in lines[4:-3]:
       ch1, ch2 = line.split('\t')
       addr = int(ch1.split(None, 2)[0], 16)
       name = ch2.split()[1]
       symbols[name] = addr
 
     # binary
```

### Comparing `supGecko-0.1.0a4/src/supGecko/gecko.py` & `supGecko-0.1.0a5/src/supGecko/gecko.py`

 * *Files identical despite different names*

### Comparing `supGecko-0.1.0a4/src/supGecko/utils.py` & `supGecko-0.1.0a5/src/supGecko/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2023 sup39
+
 def cw_addr(ct, addr, po, endif=False):
   return (ct+0x10 if po else ct)<<24 | (addr+1 if endif else addr)&0x1ff_ffff
 def cw_go(ct, if_, n):
   return ct<<24 | [True, False, None].index(if_)<<20 | n&0xffff
 
 def parse_regop(ct, lhs, op, rhs):
   if op.endswith('='): op = op[:-1] # drop trailing =
```

### Comparing `supGecko-0.1.0a4/src/supGecko.egg-info/PKG-INFO` & `supGecko-0.1.0a5/src/supGecko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supGecko
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A helper library to write Gecko code
 Home-page: https://github.com/sup39/supGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supGecko/issues
 Classifier: Programming Language :: Python :: 3
```

