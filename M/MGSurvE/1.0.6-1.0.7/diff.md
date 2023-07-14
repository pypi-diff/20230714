# Comparing `tmp/MGSurvE-1.0.6.tar.gz` & `tmp/MGSurvE-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-1.0.6.tar", last modified: Wed Jul 12 17:28:32 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.7.tar", last modified: Fri Jul 14 17:13:33 2023, max compression
```

## Comparing `MGSurvE-1.0.6.tar` & `MGSurvE-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-12 17:28:32.521221 MGSurvE-1.0.6/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/LICENSE
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-12 17:28:32.520027 MGSurvE-1.0.6/MGSurvE/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.6/MGSurvE/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.6/MGSurvE/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.6/MGSurvE/kernels.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-07-12 17:23:52.000000 MGSurvE-1.0.6/MGSurvE/landscape.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/matrices.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/network.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/optimization.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.6/MGSurvE/optimizationPSO.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-07-12 17:23:30.000000 MGSurvE-1.0.6/MGSurvE/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.6/MGSurvE/pointProcess.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-12 17:28:32.520840 MGSurvE-1.0.6/MGSurvE.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-07-12 17:28:32.000000 MGSurvE-1.0.6/MGSurvE.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-12 17:28:32.521074 MGSurvE-1.0.6/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.6/README.md
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-12 17:28:32.521280 MGSurvE-1.0.6/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.6/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 17:13:33.666114 MGSurvE-1.0.7/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 17:13:33.665049 MGSurvE-1.0.7/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.7/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.7/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.7/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21887 2023-07-14 17:12:03.000000 MGSurvE-1.0.7/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.7/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-07-12 17:23:30.000000 MGSurvE-1.0.7/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 17:13:33.665789 MGSurvE-1.0.7/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 17:13:33.665986 MGSurvE-1.0.7/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.7/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-14 17:13:33.666159 MGSurvE-1.0.7/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.7/setup.py
```

### Comparing `MGSurvE-1.0.6/LICENSE` & `MGSurvE-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/auxiliary.py` & `MGSurvE-1.0.7/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/colors.py` & `MGSurvE-1.0.7/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/constants.py` & `MGSurvE-1.0.7/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/kernels.py` & `MGSurvE-1.0.7/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/landscape.py` & `MGSurvE-1.0.7/MGSurvE/landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,17 +274,33 @@
             self.trapsKernels, self.trapsMask, self.pointTypes
         )
         ptsN = self.pointNumber
         self.trapsMigration[:ptsN, :ptsN] = np.copy(self.maskedMigration)
         self.trapsMigration[:ptsN, ptsN:] = np.copy(trapProbs)
         self.trapsMigration = normalize(self.trapsMigration, axis=1, norm='l1')
     def updateTrapsCoords(self, trapsCoords):
+        """Updates current trap coordinates.
+        
+        Parameters:
+            trapsCoords (numpy array):
+        """
         self.trapsCoords = trapsCoords
         self.calcTrapsDistances()
         self.calcTrapsMigration()
+    def updateTrapsCoordsByID(self, trapPositionsID):
+        """Updates current trap coordinates by sites ID.
+        
+        Parameters:
+            trapPositionsID (numpy array):
+        """
+        trapXY = opt.chromosomeIDtoXY(
+            trapPositionsID, self.pointID, self.pointCoords
+        )
+        self.trapsSiteID = trapPositionsID
+        self.updateTrapsCoords(trapXY)
     def updateTraps(self, traps, trapsKernels):
         """Updates the traps locations and migration matrices (in place).
 
         Parameters:
             traps (pandas dataframe):
             trapsKernel (dictionary):
         """
```

### Comparing `MGSurvE-1.0.6/MGSurvE/matrices.py` & `MGSurvE-1.0.7/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/network.py` & `MGSurvE-1.0.7/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/optimization.py` & `MGSurvE-1.0.7/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.7/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/plots.py` & `MGSurvE-1.0.7/MGSurvE/plots.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE/pointProcess.py` & `MGSurvE-1.0.7/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.7/MGSurvE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.6
+Version: 1.0.7
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.6/PKG-INFO` & `MGSurvE-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.6
+Version: 1.0.7
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.6/README.md` & `MGSurvE-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.6/setup.py` & `MGSurvE-1.0.7/setup.py`

 * *Files identical despite different names*

