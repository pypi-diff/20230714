# Comparing `tmp/antgen-0.3.9-py3-none-any.whl.zip` & `tmp/antgen-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 58696 bytes, number of entries: 115
+Zip file size: 58695 bytes, number of entries: 115
 -rw-rw-rw-  2.0 fat    18991 b- defN 23-Jul-14 16:58 antgen/ActivityModel.py
 -rw-rw-rw-  2.0 fat     5871 b- defN 23-Jul-14 16:55 antgen/ApplianceModel.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/LICENSE
 -rw-rw-rw-  2.0 fat     7913 b- defN 23-Jul-14 16:55 antgen/LoadModelComponents.py
 -rw-rw-rw-  2.0 fat     5072 b- defN 23-Jul-14 21:11 antgen/Tools.py
 -rw-rw-rw-  2.0 fat     6013 b- defN 23-Jul-14 16:55 antgen/UserModel.py
 -rw-rw-rw-  2.0 fat       76 b- defN 23-Jul-14 16:55 antgen/__init__.py
@@ -105,13 +105,13 @@
 -rw-rw-rw-  2.0 fat     8479 b- defN 23-Jul-14 16:55 antgen/appliances/TV/dev_B80E51/mode0
 -rw-rw-rw-  2.0 fat     8429 b- defN 23-Jul-14 16:55 antgen/appliances/TV/dev_B80E51/mode1
 -rw-rw-rw-  2.0 fat     7571 b- defN 23-Jul-14 16:55 antgen/appliances/TV/dev_B80E51/mode2
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/WASHINGMACHINE/ECO-H1/mode2
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/WASHINGMACHINE/_B82E27/mode0
--rw-rw-rw-  2.0 fat     1131 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    19191 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-14 21:15 antgen-0.3.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    10769 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/RECORD
-115 files, 141762 bytes uncompressed, 40812 bytes compressed:  71.2%
+-rw-rw-rw-  2.0 fat     1131 b- defN 23-Jul-14 21:41 antgen-0.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    19191 b- defN 23-Jul-14 21:41 antgen-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 21:41 antgen-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-14 21:41 antgen-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    10769 b- defN 23-Jul-14 21:41 antgen-0.4.0.dist-info/RECORD
+115 files, 141762 bytes uncompressed, 40811 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -324,23 +324,23 @@
 
 Filename: antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
 Comment: 
 
 Filename: antgen/appliances/WASHINGMACHINE/_B82E27/mode0
 Comment: 
 
-Filename: antgen-0.3.9.dist-info/LICENSE
+Filename: antgen-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: antgen-0.3.9.dist-info/METADATA
+Filename: antgen-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: antgen-0.3.9.dist-info/WHEEL
+Filename: antgen-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: antgen-0.3.9.dist-info/top_level.txt
+Filename: antgen-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: antgen-0.3.9.dist-info/RECORD
+Filename: antgen-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `antgen-0.3.9.dist-info/LICENSE` & `antgen-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `antgen-0.3.9.dist-info/METADATA` & `antgen-0.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antgen
-Version: 0.3.9
+Version: 0.4.0
 Summary: This tool generates synthetic macroscopic load signatures for their use in conjunction with NILM (load disaggregation) tools.
 Author: Nuno Velosa
 Author-email: Nuno Velosa <nunovelosa@hotmail.com>
 Project-URL: Homepage, https://gitlab.com/nunovelosa/antgen
 Project-URL: Bug Tracker, https://gitlab.com/nunovelosa/antgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `antgen-0.3.9.dist-info/RECORD` & `antgen-0.4.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -104,12 +104,12 @@
 antgen/appliances/TV/dev_B80E51/mode0,sha256=a3JQ0p4UmAeziqu76TUIE0NEgwarF8s9-V79z_WbXHg,8479
 antgen/appliances/TV/dev_B80E51/mode1,sha256=WO8fJkigYVDKJnPUHwpaDN70phKT5E4HnGPSBlBZ4T4,8429
 antgen/appliances/TV/dev_B80E51/mode2,sha256=alEsZDlZNMIV-nknaLlvugV8qdZXcZQlXNndekICV4g,7571
 antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/appliances/WASHINGMACHINE/ECO-H1/mode2,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/appliances/WASHINGMACHINE/ECO-H1/mode3,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/appliances/WASHINGMACHINE/_B82E27/mode0,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-antgen-0.3.9.dist-info/LICENSE,sha256=V3ZQ1IsxFIISGJvPm_i0oYdUGgjyadaICziDVtKoULk,1131
-antgen-0.3.9.dist-info/METADATA,sha256=LPhG_32XnG3_59yE68uMl5S8Nhlqn1zlhGoxZOtyjIU,19191
-antgen-0.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-antgen-0.3.9.dist-info/top_level.txt,sha256=lVuIG72qQlyQ93EJRsuVyiYiguJXsWRIEmfRIskw8dQ,7
-antgen-0.3.9.dist-info/RECORD,,
+antgen-0.4.0.dist-info/LICENSE,sha256=V3ZQ1IsxFIISGJvPm_i0oYdUGgjyadaICziDVtKoULk,1131
+antgen-0.4.0.dist-info/METADATA,sha256=d-a9tLDBCpKj7ovm8sle-gVFtc0_cObnQejtWkIBr6k,19191
+antgen-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+antgen-0.4.0.dist-info/top_level.txt,sha256=lVuIG72qQlyQ93EJRsuVyiYiguJXsWRIEmfRIskw8dQ,7
+antgen-0.4.0.dist-info/RECORD,,
```

