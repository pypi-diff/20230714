# Comparing `tmp/adit_dicomweb_client-0.2.0.tar.gz` & `tmp/adit_dicomweb_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adit_dicomweb_client-0.2.0.tar", max compression
+gzip compressed data, was "adit_dicomweb_client-0.3.0.tar", max compression
```

## Comparing `adit_dicomweb_client-0.2.0.tar` & `adit_dicomweb_client-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1355 2023-07-14 10:18:28.760869 adit_dicomweb_client-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-14 09:58:50.415318 adit_dicomweb_client-0.2.0/adit_dicomweb_client/__init__.py
--rw-r--r--   0        0        0     5527 2023-07-14 09:59:12.179125 adit_dicomweb_client-0.2.0/adit_dicomweb_client/adit_dicomweb_client.py
--rw-r--r--   0        0        0      399 2023-07-14 10:19:01.628579 adit_dicomweb_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 adit_dicomweb_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1350 2023-07-14 10:20:22.595866 adit_dicomweb_client-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:58:50.415318 adit_dicomweb_client-0.3.0/adit_dicomweb_client/__init__.py
+-rw-r--r--   0        0        0     5527 2023-07-14 09:59:12.179125 adit_dicomweb_client-0.3.0/adit_dicomweb_client/adit_dicomweb_client.py
+-rw-r--r--   0        0        0      399 2023-07-14 10:20:27.999818 adit_dicomweb_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 adit_dicomweb_client-0.3.0/PKG-INFO
```

### Comparing `adit_dicomweb_client-0.2.0/README.md` & `adit_dicomweb_client-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
 # Include additional query parameters
 studies = client.find_studies({"PatientID": "1001"})
 
 # Get a study
 study = client.get_study(study_instance_uid)
 
-# Retrieve a series
+# Get a series
 series = client.get_series(study_instance_uid, series_instance_uid)
 
-# Retrieve a study metadata
+# Get study metadata
 study_metadata = client.get_study_metadata(study_instance_uid)
 
-# Retrieve a series metadata
+# Get series metadata
 series_metadata = client.get_series_metadata(study_instance_uid, series_instance_uid)
 
-# Upload Dicom files
+# Upload pydicom.Dataset instances
 client.upload_instances(instance_list)
 
 
 ```
```

### Comparing `adit_dicomweb_client-0.2.0/adit_dicomweb_client/adit_dicomweb_client.py` & `adit_dicomweb_client-0.3.0/adit_dicomweb_client/adit_dicomweb_client.py`

 * *Files identical despite different names*

### Comparing `adit_dicomweb_client-0.2.0/PKG-INFO` & `adit_dicomweb_client-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adit-dicomweb-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Hummerich, Sander
 Author-email: sander.hummerich@med.uni-heidelberg.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dicomweb-client (>=0.59.1,<0.60.0)
@@ -45,21 +45,21 @@
 
 # Include additional query parameters
 studies = client.find_studies({"PatientID": "1001"})
 
 # Get a study
 study = client.get_study(study_instance_uid)
 
-# Retrieve a series
+# Get a series
 series = client.get_series(study_instance_uid, series_instance_uid)
 
-# Retrieve a study metadata
+# Get study metadata
 study_metadata = client.get_study_metadata(study_instance_uid)
 
-# Retrieve a series metadata
+# Get series metadata
 series_metadata = client.get_series_metadata(study_instance_uid, series_instance_uid)
 
-# Upload Dicom files
+# Upload pydicom.Dataset instances
 client.upload_instances(instance_list)
 
 
 ```
```

