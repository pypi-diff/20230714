# Comparing `tmp/steptools-20.4-cp37-abi3-win_amd64.whl.zip` & `tmp/steptools-20.5-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7381171 bytes, number of entries: 8
+Zip file size: 7879922 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        2 b- defN 22-Aug-19 14:38 steptools/py.typed
--rw-rw-rw-  2.0 fat 30945000 b- defN 23-Jun-28 16:48 steptools/step.pyd
+-rw-rw-rw-  2.0 fat 32872680 b- defN 23-Jul-14 00:29 steptools/step.pyd
 -rw-rw-rw-  2.0 fat   120834 b- defN 23-Jun-05 14:54 steptools/step.pyi
--rw-rw-rw-  2.0 fat     3043 b- defN 23-Jun-28 16:49 steptools-20.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7045 b- defN 23-Jun-28 16:49 steptools-20.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-28 16:49 steptools-20.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-28 16:48 steptools-20.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-Jun-28 16:49 steptools-20.4.dist-info/RECORD
-8 files, 31076659 bytes uncompressed, 7380105 bytes compressed:  76.3%
+-rw-rw-rw-  2.0 fat     3043 b- defN 23-Jul-14 00:30 steptools-20.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7045 b- defN 23-Jul-14 00:30 steptools-20.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-14 00:30 steptools-20.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-14 00:30 steptools-20.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-Jul-14 00:30 steptools-20.5.dist-info/RECORD
+8 files, 33004339 bytes uncompressed, 7878856 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: steptools/step.pyd
 Comment: 
 
 Filename: steptools/step.pyi
 Comment: 
 
-Filename: steptools-20.4.dist-info/LICENSE
+Filename: steptools-20.5.dist-info/LICENSE
 Comment: 
 
-Filename: steptools-20.4.dist-info/METADATA
+Filename: steptools-20.5.dist-info/METADATA
 Comment: 
 
-Filename: steptools-20.4.dist-info/WHEEL
+Filename: steptools-20.5.dist-info/WHEEL
 Comment: 
 
-Filename: steptools-20.4.dist-info/top_level.txt
+Filename: steptools-20.5.dist-info/top_level.txt
 Comment: 
 
-Filename: steptools-20.4.dist-info/RECORD
+Filename: steptools-20.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `steptools-20.4.dist-info/LICENSE` & `steptools-20.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `steptools-20.4.dist-info/METADATA` & `steptools-20.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steptools
-Version: 20.4
+Version: 20.5
 Summary: STEP and STEP-NC (ISO 10303) native extension for large CAD/CAM/CAE models and machine tool interfaces.
 Author-email: "STEP Tools, Inc" <support@steptools.com>
 License: 
         STEP Python Interface
         END USER LICENSE AGREEMENT
         REDISTRIBUTION NOT PERMITTED        
         STEP Tools, Inc. ("STI") grants you ("Customer") a non-exclusive,
```

## Comparing `steptools-20.4.dist-info/RECORD` & `steptools-20.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 steptools/py.typed,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-steptools/step.pyd,sha256=Sz9oDag5AhcQ00JpSKAW37qQ8wQBmyI1xXpZcmFO-cU,30945000
+steptools/step.pyd,sha256=ZA8GYTgrOf1fwZ-ducFHjXev025a3Nwme5Fg4PscnBk,32872680
 steptools/step.pyi,sha256=qmfHvNcGv5MZj_W_Mz5LmFfdmnRTfAqLo8l9NBYHiLU,120834
-steptools-20.4.dist-info/LICENSE,sha256=95amYWPb2yYw4mlPrV5p700ZxQc4vF6T7PMfLNDqqdk,3043
-steptools-20.4.dist-info/METADATA,sha256=hoVeFXvSMe-5v1Y9oIh4_5rJvmbzT1XSurwrF5NWdPs,7045
-steptools-20.4.dist-info/WHEEL,sha256=QoQ88D2Q13BOm7mJoRsoyU9fyfiVmeZqJb4AUpJxoBg,100
-steptools-20.4.dist-info/top_level.txt,sha256=makmMXVcR2PLphCyKXpEBALUpobuOltlpF-6P2Xkhas,15
-steptools-20.4.dist-info/RECORD,,
+steptools-20.5.dist-info/LICENSE,sha256=95amYWPb2yYw4mlPrV5p700ZxQc4vF6T7PMfLNDqqdk,3043
+steptools-20.5.dist-info/METADATA,sha256=99HbwPf_opIvFSGcGW8KgN5tKY0VaqPMAH9O3LeR0_4,7045
+steptools-20.5.dist-info/WHEEL,sha256=QoQ88D2Q13BOm7mJoRsoyU9fyfiVmeZqJb4AUpJxoBg,100
+steptools-20.5.dist-info/top_level.txt,sha256=makmMXVcR2PLphCyKXpEBALUpobuOltlpF-6P2Xkhas,15
+steptools-20.5.dist-info/RECORD,,
```

