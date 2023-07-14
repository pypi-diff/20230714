# Comparing `tmp/pyees-1.3.7.tar.gz` & `tmp/pyees-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.7.tar", last modified: Fri Jul 14 08:17:33 2023, max compression
+gzip compressed data, was "pyees-1.3.8.tar", last modified: Fri Jul 14 10:34:01 2023, max compression
```

## Comparing `pyees-1.3.7.tar` & `pyees-1.3.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 08:17:33.537316 pyees-1.3.7/
--rw-rw-rw-   0        0        0     1085 2023-07-14 08:17:32.954907 pyees-1.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-14 08:17:33.542302 pyees-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 08:17:33.391713 pyees-1.3.7/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.7/pyees/__init__.py
--rw-rw-rw-   0        0        0    13747 2023-07-13 16:45:15.000000 pyees-1.3.7/pyees/fit.py
--rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.3.7/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.3.7/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.7/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.3.7/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2023-07-14 08:17:33.180291 pyees-1.3.7/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-06-30 12:05:47.000000 pyees-1.3.7/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.3.7/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.7/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.7/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.3.7/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.3.7/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.3.7/pyees/testVariable.py
--rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.3.7/pyees/unit.py
--rw-rw-rw-   0        0        0    34098 2023-07-13 19:38:36.000000 pyees-1.3.7/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:17:33.518366 pyees-1.3.7/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-14 08:17:33.564242 pyees-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-14 08:17:22.000000 pyees-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:34:01.900036 pyees-1.3.8/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-14 10:34:01.907020 pyees-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 10:34:01.767378 pyees-1.3.8/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.8/pyees/__init__.py
+-rw-rw-rw-   0        0        0    14756 2023-07-14 10:33:08.000000 pyees-1.3.8/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.3.8/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.3.8/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.3.8/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.8/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.3.8/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.8/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7661 2023-07-14 10:08:51.000000 pyees-1.3.8/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.3.8/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.8/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.8/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.3.8/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.3.8/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.3.8/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.3.8/pyees/unit.py
+-rw-rw-rw-   0        0        0    34114 2023-07-14 10:18:19.000000 pyees-1.3.8/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:34:01.885075 pyees-1.3.8/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-14 10:34:00.000000 pyees-1.3.8/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-14 10:34:01.000000 pyees-1.3.8/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 10:34:00.000000 pyees-1.3.8/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 10:34:00.000000 pyees-1.3.8/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 10:34:01.000000 pyees-1.3.8/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-14 10:34:01.931955 pyees-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-14 10:33:55.000000 pyees-1.3.8/setup.py
```

### Comparing `pyees-1.3.7/LICENSE.txt` & `pyees-1.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/PKG-INFO` & `pyees-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.7
+Version: 1.3.8
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.7/README.md` & `pyees-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/fit.py` & `pyees-1.3.8/pyees/fit.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,38 @@
         self.xVal = x.value
         self.yVal = y.value
         self.xUnit = x._unitObject
         self.yUnit = y._unitObject
         self.xUncert = x.uncert
         self.yUncert = y.uncert
 
+
+        indexesNotToUse = []
+        for i in range(len(self.xVal)):
+            if np.isnan(self.xVal[i]):
+                indexesNotToUse.append(i)
+                continue
+            if np.isnan(self.xUncert[i]):
+                indexesNotToUse.append(i)
+                continue
+            if np.isnan(self.yVal[i]):
+                indexesNotToUse.append(i)
+                continue
+            if np.isnan(self.yUncert[i]):
+                indexesNotToUse.append(i)
+                continue
+        
+
+        if indexesNotToUse:
+            indexesToUse = [i for i in range(len(self.xVal)) if not i in indexesNotToUse]
+            self.xVal = self.xVal[indexesToUse]
+            self.xUncert = self.xUncert[indexesToUse]
+            self.yVal = self.yVal[indexesToUse]
+            self.yUncert = self.yUncert[indexesToUse]
+
         # uncertanties can not be 0
         if len(self.xVal) == 1:
             self._sx = self.xUncert if self.xUncert != 0 else 1e-10
         else:
             self._sx = [elem if elem != 0 else 1e-10 for elem in self.xUncert]
         if len(self.yVal) == 1:
             self._sy = self.yUncert if self.yUncert != 0 else 1e-10
@@ -63,19 +87,19 @@
                 self.coefficients[i].addCovariance(
                     var = self.coefficients[j],
                     covariance = regression.cov_beta[i,j],
                     unitStr = str(self.coefficients[i]._unitObject * self.coefficients[j]._unitObject)
                 )
 
         # determine r-squared
-        self._residuals = y - self._predict(x)
+        self._residuals = np.array([yi - pi for yi, pi in zip(self.yVal, self._predict(regression.beta, self.xVal))])# y.value - self._predict(x.value)
         ss_res = sum(self._residuals**2)
-        ss_tot = sum((y - np.mean(y))**2)
+        ss_tot = sum((self.yVal - np.mean(self.yVal))**2)
         if ss_tot != 0:
-            self.r_squared = 1 - (ss_res / ss_tot)
+            self.r_squared = variable(1 - (ss_res / ss_tot))
         else:
             self.r_squared = variable(1)
         np.seterr('warn')
 
     def __str__(self):
         return self.func_name() + ',  ' + self._r2_name()
 
@@ -158,18 +182,18 @@
         ax.plot(self.xVal, self.yVal, label=label, **kwargs)
 
     def predict(self, x):
         if not isinstance(x, scalarVariable):
             raise ValueError('The input "x" has to be a variable')
         return self.func(x)
     
-    def _predict(self, x):
-        if not isinstance(x, scalarVariable):
-            x = variable(x, self.xUnit)
-        return self.func(x)
+    def _predict(self, coeffs, x):
+        # if not isinstance(x, scalarVariable):
+        #     x = variable(x, self.xUnit)
+        return self._func(coeffs, x)
 
     def plotUncertanty(self, ax, x = None, **kwargs):
         
         if x is None:
             x = variable(np.linspace(np.min(self.xVal), np.max(self.xVal), 100), self.xUnit)
         else:
             if not isinstance(x, arrayVariable):
```

### Comparing `pyees-1.3.7/pyees/profilePyees.py` & `pyees-1.3.8/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/prop.py` & `pyees-1.3.8/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/sheet.py` & `pyees-1.3.8/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/solve.py` & `pyees-1.3.8/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/stackOverflowODR.py` & `pyees-1.3.8/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/testFit.py` & `pyees-1.3.8/pyees/testFit.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
         # ## TODO compare this to the example in the book
         # fig2, ax2 = plt.subplots()
         # fit.plotNormalizedResiduals(ax2, label = 'normalized resudials')
         # np.testing.assert_array_equal(ax2.lines[0].get_ydata(), [])
 
-        
+
         
         
 
     def testLinFit(self):
         a = 2
         b = 10
         n = 100
```

### Comparing `pyees-1.3.7/pyees/testProp.py` & `pyees-1.3.8/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/testPyees.py` & `pyees-1.3.8/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/testSheet.py` & `pyees-1.3.8/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/testSolve.py` & `pyees-1.3.8/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/testUnit.py` & `pyees-1.3.8/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/testVariable.py` & `pyees-1.3.8/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/unit.py` & `pyees-1.3.8/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.7/pyees/variable.py` & `pyees-1.3.8/pyees/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         value, uncert = self.printUncertanty(value, uncert)
         if uncert is None:
             return rf'{value}{space}{unitStr}'
         else:
                 return rf'{value} {pm} {uncert}{space}{unitStr}'
 
     def _addDependent(self, var, grad):
-                
+                                
         # scale the gradient to SI units. This is necessary if one of the variables are converted after the dependency has been noted
         grad *= self._converterToSI.convert(1, useOffset=False) / var._converterToSI.convert(1, useOffset=False)
         
         if var.dependsOn:
             # the variable depends on other variables
             # loop over the dependencies of the variables and add them to the dependencies of self.
             # this ensures that the product rule is used
```

### Comparing `pyees-1.3.7/pyees.egg-info/PKG-INFO` & `pyees-1.3.8/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.7
+Version: 1.3.8
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.7/setup.py` & `pyees-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.7',
+    version='1.3.8',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

