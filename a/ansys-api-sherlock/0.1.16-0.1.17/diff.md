# Comparing `tmp/ansys-api-sherlock-0.1.16.tar.gz` & `tmp/ansys-api-sherlock-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-sherlock-0.1.16.tar", last modified: Wed Jul  5 21:35:57 2023, max compression
+gzip compressed data, was "ansys-api-sherlock-0.1.17.tar", last modified: Fri Jul 14 17:40:06 2023, max compression
```

## Comparing `ansys-api-sherlock-0.1.16.tar` & `ansys-api-sherlock-0.1.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.564049 ansys-api-sherlock-0.1.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-05 21:35:57.564049 ansys-api-sherlock-0.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:35:57.564049 ansys-api-sherlock-0.1.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.560049 ansys-api-sherlock-0.1.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.560049 ansys-api-sherlock-0.1.16/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.560049 ansys-api-sherlock-0.1.16/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.560049 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.564049 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockCommonService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockLayerService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockModelService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockPartsService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockProjectService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-05 21:35:37.000000 ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockStackupService.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:35:57.564049 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-05 21:35:57.000000 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 21:35:57.000000 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:35:57.000000 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 21:35:57.000000 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 21:35:57.000000 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 21:35:57.000000 ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.172834 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockCommonService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLayerService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockModelService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockPartsService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockProjectService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-14 17:39:49.000000 ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockStackupService.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:40:06.176834 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 17:40:06.000000 ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/top_level.txt
```

### Comparing `ansys-api-sherlock-0.1.16/LICENSE` & `ansys-api-sherlock-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/PKG-INFO` & `ansys-api-sherlock-0.1.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.16
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 21:35:57 on 05 July 2023
+Version: 0.1.17
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 17:40:06 on 14 July 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.16/README.md` & `ansys-api-sherlock-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/setup.py` & `ansys-api-sherlock-0.1.17/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockCommonService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockCommonService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockLayerService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLayerService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockModelService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockModelService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockPartsService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockPartsService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockProjectService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockProjectService.proto`

 * *Files 15% similar despite different names*

```diff
@@ -138,14 +138,30 @@
   message CCA {
     string ccaName				= 1;	// Name of the CCA.
     repeated CCA subAssemblies	= 2;	// Sub-assemblies assigned to the CCA.
   }
   repeated CCA ccas				= 2;	// CCA's assigned to the project.
 }
 
+message CCA {
+  string ccaName = 1; 									// Name of the Circuit Card
+  optional string description = 2; 						// Description of the circuit card
+  optional string defaultSolderType = 3; 				// Default solder type
+  optional double defaultStencilThickness = 4; 			// Default stencil thickness
+  optional string defaultStencilThicknessUnits = 5; 	// Default stencil thickness units
+  optional double defaultPartTempRise = 6; 				// Default part temp rise
+  optional string defaultPartTempRiseUnits = 7; 		// Default part temp rise units
+  optional bool guessPartPropertiesEnabled = 8; 		// Whether to enable guess part properties
+}
+
+message AddCcaRequest {
+  string project = 1;		// Name of the project
+  repeated CCA CCAs = 2;	// CCAs to add
+}
+
 service SherlockProjectService {
   // Generates the project report and return it via streaming.
   rpc genReport(GenReportRequest) returns (stream GenReportResponse);
 
   // Generates the project CCA report and return it via streaming.
   rpc genCCAReport(GenCCAReportRequest) returns (stream GenCCAReportResponse);
   
@@ -162,8 +178,11 @@
   rpc addStrainMap(AddStrainMapRequest) returns (AddStrainMapResponse);
   
    // Returns a list of circuit cards and their assigned strain maps for a given Sherlock project.
   rpc listStrainMaps(ListStrainMapsRequest) returns (ListStrainMapsResponse);
 
    // Returns a list of circuit cards, their properties, and sub-assemblies for a given Sherlock project.
   rpc listCCAs(ListCCAsRequest) returns (ListCCAsResponse);
+  
+  // Creates a new circuit card assembly.
+  rpc addCCA(AddCcaRequest) returns (ReturnCode);
 }
```

### Comparing `ansys-api-sherlock-0.1.16/src/ansys/api/sherlock/v0/SherlockStackupService.proto` & `ansys-api-sherlock-0.1.17/src/ansys/api/sherlock/v0/SherlockStackupService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/PKG-INFO` & `ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.16
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 21:35:57 on 05 July 2023
+Version: 0.1.17
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 17:40:06 on 14 July 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.16/src/ansys_api_sherlock.egg-info/SOURCES.txt` & `ansys-api-sherlock-0.1.17/src/ansys_api_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

