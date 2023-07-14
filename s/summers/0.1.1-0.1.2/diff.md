# Comparing `tmp/summers-0.1.1-py3-none-any.whl.zip` & `tmp/summers-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7907 bytes, number of entries: 9
+Zip file size: 7909 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx     3225 b- defN 23-Jul-14 10:41 summers/__init__.py
 -rw-rw-r--  2.0 unx      354 b- defN 23-Jul-14 10:41 summers/cc.py
 -rw-rw-r--  2.0 unx     3371 b- defN 23-Jul-14 10:41 summers/di.py
 -rw-rw-r--  2.0 unx     1996 b- defN 23-Jul-14 10:41 summers/sc_imp.py
 -rw-rw-r--  2.0 unx     4092 b- defN 23-Jul-14 10:41 summers/sc_txt.py
--rw-rw-r--  2.0 unx     4058 b- defN 23-Jul-14 10:56 summers-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-14 10:56 summers-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jul-14 10:56 summers-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      660 b- defN 23-Jul-14 10:56 summers-0.1.1.dist-info/RECORD
-9 files, 17856 bytes uncompressed, 6787 bytes compressed:  62.0%
+-rw-rw-r--  2.0 unx     4058 b- defN 23-Jul-14 10:58 summers-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-14 10:58 summers-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-14 10:58 summers-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      660 b- defN 23-Jul-14 10:58 summers-0.1.2.dist-info/RECORD
+9 files, 17856 bytes uncompressed, 6789 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: summers/sc_imp.py
 Comment: 
 
 Filename: summers/sc_txt.py
 Comment: 
 
-Filename: summers-0.1.1.dist-info/METADATA
+Filename: summers-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: summers-0.1.1.dist-info/WHEEL
+Filename: summers-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: summers-0.1.1.dist-info/top_level.txt
+Filename: summers-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: summers-0.1.1.dist-info/RECORD
+Filename: summers-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `summers-0.1.1.dist-info/METADATA` & `summers-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: summers
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个 python 依赖注入框架 <A dependency injection toolkit like Spring (java framework)>
 Home-page: https://github.com/tuijs/summers
 Author: weiyi
 Author-email: 272654394@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `summers-0.1.1.dist-info/RECORD` & `summers-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 summers/__init__.py,sha256=-fggyGoWCQPgDwbwvAvgwyDtl5wZBdQyImpyWEprdmk,3225
 summers/cc.py,sha256=L1jCssoO0_YD0U2pxgBHFQdlnmVX6z3ZYEt36Gd9Kv4,354
 summers/di.py,sha256=idT-D_hOZCfeU6dppbuEiOJP_Zs7i867eLIYHWxQ0WA,3371
 summers/sc_imp.py,sha256=Q08Srd29Sfa5hnhdqsTetfX7yweYmD96YmARbWqzT4I,1996
 summers/sc_txt.py,sha256=siQUPEg5TFuOfRlavKRlllLRfpfWD2qfsUSOspfMV7I,4092
-summers-0.1.1.dist-info/METADATA,sha256=IV5Of5jtF_6P7GLymwQFPGYpAjosXqeBmparV0pPo_Q,4058
-summers-0.1.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-summers-0.1.1.dist-info/top_level.txt,sha256=k6Qomaj62_zErR8OF1SCi5dxZXAMHqM8Ayr27DcWJC0,8
-summers-0.1.1.dist-info/RECORD,,
+summers-0.1.2.dist-info/METADATA,sha256=CD-K_FhZJmTOR-gWa7IfpcfenKk99HwK5oBCwXzNxBs,4058
+summers-0.1.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+summers-0.1.2.dist-info/top_level.txt,sha256=k6Qomaj62_zErR8OF1SCi5dxZXAMHqM8Ayr27DcWJC0,8
+summers-0.1.2.dist-info/RECORD,,
```

