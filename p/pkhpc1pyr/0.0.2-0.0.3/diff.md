# Comparing `tmp/pkhpc1pyr-0.0.2.tar.gz` & `tmp/pkhpc1pyr-0.0.3.tar.gz`

## Comparing `pkhpc1pyr-0.0.2.tar` & `pkhpc1pyr-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/requirements.txt
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L1.py
--rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L2.py
--rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L3.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/__init__.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L1.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L2.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L3.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Err.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Plot.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Err.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Plot.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Err.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Plot.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/helperFunctions.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/LICENSE
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L1.py
+-rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L2.py
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L3.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/__init__.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L1.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L2.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L3.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Err.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Plot.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Err.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Plot.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Err.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Plot.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/helperFunctions.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/PKG-INFO
```

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L1.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L1.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L2.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L2.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L3.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L3.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,16 +167,16 @@
                 # Total signal at the end of TR equals the IC for the next TR
                 MzevSegIC = np.matmul( P,(MzevSeg1 + kvedve*(MzevSeg2a+MzevSeg2b)) )
 
         if fdv['NSeg'] > 1:
             # In version 0.0.1, fdv['NSeg']>1 is not supported
             print('Segmented acquisition not set up yet')
         else:
-            Mxyev[:,i-1] = np.reshape( MxyevSeg, (4,) )
-            Mzev[:, i-1] = np.reshape( MzevSeg, (4,) )
+            Mxyev[:,i] = np.reshape( MxyevSeg, (4,) )
+            Mzev[:, i] = np.reshape( MzevSeg, (4,) )
 
             Mxyiv[:, i] = MxyivSeg[:, i]
             Mziv[:, i] = MzivSeg[:, i]
     ### END OF CALCULATION LOOP ###
 
     if fdv['verbose']:
```

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L1.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L1.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L2.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L2.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,15 +90,18 @@
         parms = np.array( parms )
     EV, IV, vb, Mzev, Mziv = P2L2(parms, fdv) 
     fdv['data'] = IV*vb + EV*(1-vb)
 
     ### Create a fit for the generated data and try to recover parameters above ###
     LB = [0, 0]
     UB = [1, np.Inf]
-    guess = (parms*10) * np.random.rand(2)
+
+    guess = parms
+    guess[0] = (UB[0]/guess[0]) * np.random.rand(1) * guess[0]
+    guess[1] = 2 * np.random.rand(1) * guess[1]
 
     # Optimize parameters by solving least squares problem for residuals
     fit = opt.least_squares(
         fun = P2L2Err.P2L2ErrOuter(fdv),
         x0 = guess,
         bounds = (LB, UB)
     )
```

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L3.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L3.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,24 +86,27 @@
         fdv['VIFL'] = np.zeros( (1, fdv['NFlips']) )
 
     # Placeholder data to be fit
     fdv['data'] = np.ones( (2, fdv['ntp']) )
 
     # Generate synthetic data
     if parms == None:
-        parms = np.array( [0.1, 1000] )
+        parms = np.array( [0.5, 1000] )
     else:
         parms = np.array(parms)
     EV, IV, vols, Mzev, Mziv = P2L3(parms, fdv)
     fdv['data'] = IV[0:2]*vols[0] + EV[0:2]*vols[1] + EV[2:4]*vols[2]
 
     ### Create a fit for the generated data and try to recover parameters above ###
     LB = [0,0]
     UB = [1, np.Inf]
-    guess = (parms*10) * np.random.rand(2)
+    
+    guess=parms
+    guess[0] = (UB[0] / guess[0]) * np.random.rand(1) * guess[0]
+    guess[1] = guess[1] * np.random.rand(1) * 2
 
     # Optimize parameters by solving least squares problem for residuals
     fit = opt.least_squares(
         fun = P2L3Err.P2L3ErrOuter(fdv),
         x0 = guess,
         bounds = (LB, UB)
     )
```

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Err.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Plot.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Plot.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Err.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Plot.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Plot.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Err.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Plot.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Plot.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/helperFunctions.py` & `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/helperFunctions.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/LICENSE` & `pkhpc1pyr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/README.md` & `pkhpc1pyr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.2/pyproject.toml` & `pkhpc1pyr-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pkhpc1pyr"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ryan Boyce", email="ryty.boyce@gmail.com" },
 ]
 description = "Scripts and functions for the pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate."
 readme = "README.md"
 requires-python = "~=3.10"
 classifiers = [
```

### Comparing `pkhpc1pyr-0.0.2/PKG-INFO` & `pkhpc1pyr-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkhpc1pyr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scripts and functions for the pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate.
 Project-URL: Homepage, https://github.com/RytyB/HP-C1Pyr-PK-Python
 Author-email: Ryan Boyce <ryty.boyce@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

