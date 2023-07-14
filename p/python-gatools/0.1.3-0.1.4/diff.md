# Comparing `tmp/python_gatools-0.1.3-py3-none-any.whl.zip` & `tmp/python_gatools-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,22 @@
-Zip file size: 3710 bytes, number of entries: 8
--rw-r--r--  2.0 unx       84 b- defN 23-Jul-04 16:45 gatools/__init__.py
--rw-r--r--  2.0 unx      173 b- defN 23-Jul-04 16:45 gatools/envs.py
--rw-r--r--  2.0 unx      419 b- defN 23-Jul-04 16:45 gatools/files.py
--rw-r--r--  2.0 unx     4899 b- defN 23-Jul-04 16:45 gatools/logger.py
--rw-r--r--  2.0 unx      271 b- defN 23-Jul-04 16:45 python_gatools-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 16:45 python_gatools-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-04 16:45 python_gatools-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      615 b- defN 23-Jul-04 16:45 python_gatools-0.1.3.dist-info/RECORD
-8 files, 6561 bytes uncompressed, 2634 bytes compressed:  59.9%
+Zip file size: 20109 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      463 b- defN 23-Jul-14 03:25 gatools/__init__.py
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-14 03:25 gatools/colors.py
+-rw-r--r--  2.0 unx    17593 b- defN 23-Jul-14 03:25 gatools/commons.py
+-rw-r--r--  2.0 unx      421 b- defN 23-Jul-14 03:25 gatools/ctxman.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Jul-14 03:25 gatools/decorators.py
+-rw-r--r--  2.0 unx     1416 b- defN 23-Jul-14 03:25 gatools/dictkeys.py
+-rw-r--r--  2.0 unx      618 b- defN 23-Jul-14 03:25 gatools/dictops.py
+-rw-r--r--  2.0 unx      173 b- defN 23-Jul-14 03:25 gatools/envs.py
+-rw-r--r--  2.0 unx      562 b- defN 23-Jul-14 03:25 gatools/files.py
+-rw-r--r--  2.0 unx     1172 b- defN 23-Jul-14 03:25 gatools/jsonencoder.py
+-rw-r--r--  2.0 unx     4899 b- defN 23-Jul-14 03:25 gatools/logger.py
+-rw-r--r--  2.0 unx     5120 b- defN 23-Jul-14 03:25 gatools/oar.py
+-rw-r--r--  2.0 unx     9129 b- defN 23-Jul-14 03:25 gatools/pyplot.py
+-rw-r--r--  2.0 unx     2251 b- defN 23-Jul-14 03:25 gatools/tables.py
+-rw-r--r--  2.0 unx     1640 b- defN 23-Jul-14 03:25 gatools/temp.py
+-rw-r--r--  2.0 unx     2807 b- defN 23-Jul-14 03:25 gatools/utils.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1509 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/RECORD
+20 files, 51785 bytes uncompressed, 17699 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,25 +1,61 @@
 Filename: gatools/__init__.py
 Comment: 
 
+Filename: gatools/colors.py
+Comment: 
+
+Filename: gatools/commons.py
+Comment: 
+
+Filename: gatools/ctxman.py
+Comment: 
+
+Filename: gatools/decorators.py
+Comment: 
+
+Filename: gatools/dictkeys.py
+Comment: 
+
+Filename: gatools/dictops.py
+Comment: 
+
 Filename: gatools/envs.py
 Comment: 
 
 Filename: gatools/files.py
 Comment: 
 
+Filename: gatools/jsonencoder.py
+Comment: 
+
 Filename: gatools/logger.py
 Comment: 
 
-Filename: python_gatools-0.1.3.dist-info/METADATA
+Filename: gatools/oar.py
+Comment: 
+
+Filename: gatools/pyplot.py
+Comment: 
+
+Filename: gatools/tables.py
+Comment: 
+
+Filename: gatools/temp.py
+Comment: 
+
+Filename: gatools/utils.py
+Comment: 
+
+Filename: python_gatools-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: python_gatools-0.1.3.dist-info/WHEEL
+Filename: python_gatools-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: python_gatools-0.1.3.dist-info/top_level.txt
+Filename: python_gatools-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: python_gatools-0.1.3.dist-info/RECORD
+Filename: python_gatools-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gatools/__init__.py

```diff
@@ -1,3 +1,14 @@
 from gatools.logger import *
 from gatools.envs import *
 from gatools.files import *
+from gatools.colors import Color
+from gatools.ctxman import timeout
+from gatools.decorators import *
+from gatools.utils import *
+from gatools.jsonencoder import *
+from gatools.dictkeys import print_keys
+from gatools.dictops import analyse, query
+from gatools.pyplot import *
+from gatools.tables import Table
+from gatools.temp import TmpDir, TmpFile
+from gatools.commons import *
```

## gatools/files.py

```diff
@@ -1,17 +1,22 @@
 import os
 import pathlib
 
-__ALL__ = ["Tree", "fTree"]
+__ALL__ = ["Tree", "fTree", "removeIfExists"]
 
 
 class Tree(type(pathlib.Path())):
     def mkdir(self, parents=True, exist_ok=True):
         super().mkdir(parents=parents, exist_ok=exist_ok)
 
 
 class fTree(Tree):
     def __new__(cls, *args, **kwargs):
         args = list(args)
         if (x := pathlib.Path(args[0])).is_file():
             args[0] = x.parent
         return super().__new__(cls, *args, **kwargs)
+
+def removeIfExists(fname: str):
+    """Remove `fname` if it exists"""
+    if os.path.exists(fname):
+        os.remove(fname)
```

