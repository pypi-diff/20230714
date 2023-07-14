# Comparing `tmp/abeja_sdk-2.2.1-py3-none-any.whl.zip` & `tmp/abeja_sdk-2.2.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 97759 bytes, number of entries: 93
+Zip file size: 97792 bytes, number of entries: 93
 -rw-r--r--  2.0 unx      200 b- defN 80-Jan-01 00:00 abeja/__init__.py
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 abeja/base_client.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/common/__init__.py
 -rw-r--r--  2.0 unx      406 b- defN 80-Jan-01 00:00 abeja/common/api_client.py
 -rw-r--r--  2.0 unx     2063 b- defN 80-Jan-01 00:00 abeja/common/auth.py
 -rw-r--r--  2.0 unx      714 b- defN 80-Jan-01 00:00 abeja/common/config.py
 -rw-r--r--  2.0 unx     8053 b- defN 80-Jan-01 00:00 abeja/common/connection.py
@@ -83,13 +83,13 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/training/py.typed
 -rw-r--r--  2.0 unx     2981 b- defN 80-Jan-01 00:00 abeja/training/statistics.py
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 abeja/triggers/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/triggers/api/__init__.py
 -rw-r--r--  2.0 unx    14857 b- defN 80-Jan-01 00:00 abeja/triggers/api/client.py
 -rw-r--r--  2.0 unx       51 b- defN 80-Jan-01 00:00 abeja/user/__init__.py
 -rw-r--r--  2.0 unx     1601 b- defN 80-Jan-01 00:00 abeja/user/user.py
--rw-r--r--  2.0 unx      152 b- defN 80-Jan-01 00:00 abeja/version.py
--rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abeja_sdk-2.2.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1431 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     7623 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1.dist-info/RECORD
-93 files, 485415 bytes uncompressed, 85745 bytes compressed:  82.3%
+-rw-r--r--  2.0 unx      155 b- defN 80-Jan-01 00:00 abeja/version.py
+-rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1434 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/METADATA
+?rw-r--r--  2.0 unx     7635 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/RECORD
+93 files, 485433 bytes uncompressed, 85754 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -261,20 +261,20 @@
 
 Filename: abeja/user/user.py
 Comment: 
 
 Filename: abeja/version.py
 Comment: 
 
-Filename: abeja_sdk-2.2.1.dist-info/LICENSE
+Filename: abeja_sdk-2.2.1rc1.dist-info/LICENSE
 Comment: 
 
-Filename: abeja_sdk-2.2.1.dist-info/WHEEL
+Filename: abeja_sdk-2.2.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: abeja_sdk-2.2.1.dist-info/METADATA
+Filename: abeja_sdk-2.2.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: abeja_sdk-2.2.1.dist-info/RECORD
+Filename: abeja_sdk-2.2.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abeja/version.py

```diff
@@ -1,3 +1,3 @@
 # The VERSION value is rewritten by CI to the correct value at the time of deployment.
 # see: ${REPOSITORY_ROOT}/.circleci/config.yml
-VERSION = "2.2.1"
+VERSION = "2.2.1rc1"
```

## Comparing `abeja_sdk-2.2.1.dist-info/LICENSE` & `abeja_sdk-2.2.1rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `abeja_sdk-2.2.1.dist-info/METADATA` & `abeja_sdk-2.2.1rc1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abeja-sdk
-Version: 2.2.1
+Version: 2.2.1rc1
 Summary: ABEJA Platform Software Development Kit
 License: Apache-2.0
 Author: ABEJA Inc.
 Author-email: platform-support@abejainc.com
 Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `abeja_sdk-2.2.1.dist-info/RECORD` & `abeja_sdk-2.2.1rc1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -82,12 +82,12 @@
 abeja/training/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/training/statistics.py,sha256=srEprLDKZSSTmgI3g7rBbDxQzFkDg8FN5OTFH1muwfU,2981
 abeja/triggers/__init__.py,sha256=1juY5YZuLTVcG2h614iwS16NiO-7xuEl62tEe-Hf56A,63
 abeja/triggers/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/triggers/api/client.py,sha256=ftNmiw7fxu43ChUCeNlieKUc3NNIUUccXI6AlDFDIX0,14857
 abeja/user/__init__.py,sha256=js-XQZRHXsGJZ-r9H-cLGQKa_YXmjjPmklnVe9Y12D8,51
 abeja/user/user.py,sha256=KAILiaZ1QaS2gMzFl2Vb1sBdhjKKctv8PYA6jDc1Two,1601
-abeja/version.py,sha256=41suXbsRBTZxEGpxEbNYIkEvpZSmO1fsu6qmeoyEqe8,152
-abeja_sdk-2.2.1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
-abeja_sdk-2.2.1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-abeja_sdk-2.2.1.dist-info/METADATA,sha256=KPOH_AArqZ-7Z0VlPEadZmki3a_kS1ZlU4aOoOSKkP0,1431
-abeja_sdk-2.2.1.dist-info/RECORD,,
+abeja/version.py,sha256=xfnGUXB-jD1ysWId5dygDFb3Y1dFSo4HbzQaWOV00VQ,155
+abeja_sdk-2.2.1rc1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
+abeja_sdk-2.2.1rc1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+abeja_sdk-2.2.1rc1.dist-info/METADATA,sha256=v0dt2rEu8k6dgCUsqb9yQFMMBYEpz15HAQpKT9qKej4,1434
+abeja_sdk-2.2.1rc1.dist-info/RECORD,,
```

