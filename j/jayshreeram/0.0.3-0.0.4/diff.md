# Comparing `tmp/jayshreeram-0.0.3-py3-none-any.whl.zip` & `tmp/jayshreeram-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 1408 bytes, number of entries: 5
--rw-r--r--  2.0 unx      113 b- defN 23-Jul-14 18:25 jayshreeram/__init__.py
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      392 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/RECORD
-5 files, 921 bytes uncompressed, 672 bytes compressed:  27.0%
+Zip file size: 1690 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      141 b- defN 23-Jul-14 18:38 jayshreeram/__init__.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-14 18:41 jayshreeram-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 18:41 jayshreeram-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-14 18:41 jayshreeram-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-14 18:41 jayshreeram-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      491 b- defN 23-Jul-14 18:41 jayshreeram-0.0.4.dist-info/RECORD
+6 files, 1107 bytes uncompressed, 790 bytes compressed:  28.6%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
 Filename: jayshreeram/__init__.py
 Comment: 
 
-Filename: jayshreeram-0.0.3.dist-info/METADATA
+Filename: jayshreeram-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: jayshreeram-0.0.3.dist-info/WHEEL
+Filename: jayshreeram-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: jayshreeram-0.0.3.dist-info/top_level.txt
+Filename: jayshreeram-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: jayshreeram-0.0.3.dist-info/RECORD
+Filename: jayshreeram-0.0.4.dist-info/top_level.txt
+Comment: 
+
+Filename: jayshreeram-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jayshreeram/__init__.py

```diff
@@ -1,5 +1,7 @@
 import sys
 
-print("॥ जय श्री राम ॥")
-for i in range(len(sys.argv)):
-    print(sys.argv[i])
+def display():
+    print("॥ जय श्री राम ॥")
+
+    for i in range(len(sys.argv)):
+        print(sys.argv[i])
```

