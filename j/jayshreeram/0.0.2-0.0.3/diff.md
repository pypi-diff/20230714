# Comparing `tmp/jayshreeram-0.0.2-py3-none-any.whl.zip` & `tmp/jayshreeram-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1363 bytes, number of entries: 5
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-14 18:06 jayshreeram/__init__.py
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-14 18:07 jayshreeram-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 18:07 jayshreeram-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-14 18:07 jayshreeram-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      391 b- defN 23-Jul-14 18:07 jayshreeram-0.0.2.dist-info/RECORD
-5 files, 868 bytes uncompressed, 627 bytes compressed:  27.8%
+Zip file size: 1408 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      113 b- defN 23-Jul-14 18:25 jayshreeram/__init__.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      392 b- defN 23-Jul-14 18:26 jayshreeram-0.0.3.dist-info/RECORD
+5 files, 921 bytes uncompressed, 672 bytes compressed:  27.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jayshreeram/__init__.py
 Comment: 
 
-Filename: jayshreeram-0.0.2.dist-info/METADATA
+Filename: jayshreeram-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: jayshreeram-0.0.2.dist-info/WHEEL
+Filename: jayshreeram-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: jayshreeram-0.0.2.dist-info/top_level.txt
+Filename: jayshreeram-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: jayshreeram-0.0.2.dist-info/RECORD
+Filename: jayshreeram-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jayshreeram/__init__.py

```diff
@@ -1,2 +1,5 @@
+import sys
+
 print("॥ जय श्री राम ॥")
-print("Hello")
+for i in range(len(sys.argv)):
+    print(sys.argv[i])
```

