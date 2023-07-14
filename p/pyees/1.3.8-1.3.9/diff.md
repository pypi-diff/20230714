# Comparing `tmp/pyees-1.3.8.tar.gz` & `tmp/pyees-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.8.tar", last modified: Fri Jul 14 10:34:01 2023, max compression
+gzip compressed data, was "pyees-1.3.9.tar", last modified: Fri Jul 14 10:43:20 2023, max compression
```

## Comparing `pyees-1.3.8.tar` & `pyees-1.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 10:34:01.900036 pyees-1.3.8/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-14 10:34:01.907020 pyees-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 10:34:01.767378 pyees-1.3.8/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.8/pyees/__init__.py
--rw-rw-rw-   0        0        0    14756 2023-07-14 10:33:08.000000 pyees-1.3.8/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.3.8/pyees/profileFit.py
--rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.3.8/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.3.8/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.8/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.3.8/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.8/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7661 2023-07-14 10:08:51.000000 pyees-1.3.8/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.3.8/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.8/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.8/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.3.8/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.3.8/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.3.8/pyees/testVariable.py
--rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.3.8/pyees/unit.py
--rw-rw-rw-   0        0        0    34114 2023-07-14 10:18:19.000000 pyees-1.3.8/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:34:01.885075 pyees-1.3.8/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-14 10:34:00.000000 pyees-1.3.8/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-14 10:34:01.000000 pyees-1.3.8/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 10:34:00.000000 pyees-1.3.8/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-14 10:34:00.000000 pyees-1.3.8/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 10:34:01.000000 pyees-1.3.8/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-14 10:34:01.931955 pyees-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-14 10:33:55.000000 pyees-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:43:20.067441 pyees-1.3.9/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-14 10:43:20.596026 pyees-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 10:43:20.463382 pyees-1.3.9/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.9/pyees/__init__.py
+-rw-rw-rw-   0        0        0    14848 2023-07-14 10:40:42.000000 pyees-1.3.9/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.3.9/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.3.9/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.3.9/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.9/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.3.9/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.9/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-07-14 10:43:20.288849 pyees-1.3.9/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.3.9/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.9/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.9/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.3.9/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.3.9/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.3.9/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.3.9/pyees/unit.py
+-rw-rw-rw-   0        0        0    34114 2023-07-14 10:43:20.478343 pyees-1.3.9/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:43:20.576083 pyees-1.3.9/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 10:43:19.000000 pyees-1.3.9/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-14 10:43:20.623952 pyees-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-14 10:43:18.000000 pyees-1.3.9/setup.py
```

### Comparing `pyees-1.3.8/LICENSE.txt` & `pyees-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/PKG-INFO` & `pyees-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.8
+Version: 1.3.9
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.8/README.md` & `pyees-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/fit.py` & `pyees-1.3.9/pyees/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,31 +295,31 @@
     def _func(self, x):
         return 1
 
     def func_name(self):
         return f'{self.popt[0]}'
 
 class exp_fit(_fit):
-    def __init__(self, x, y, p0=[1, 1]):
-        if len(p0) != 2:
-            raise ValueError('You have to provide initial guesses for 2 parameters')
+    def __init__(self, x, y, p0=[1, 1, 1, 1]):
+        if len(p0) != 4:
+            raise ValueError('You have to provide initial guesses for 4 parameters')
         if x.unit != '1':
             raise ValueError('The variable "x" cannot have a unit')
         _fit.__init__(self, self.func, x, y, p0=p0)
 
     def getVariableUnits(self):
-        return [self.yUnit, '']
+        return [self.yUnit, '', '', self.yUnit]
 
     def _func(self, B, x):
-        a = B[0]
-        b = B[1]
-        return a * b**x
+        a,b,c,d = B
+        return a * b**(x-c) + d
 
     def func_name(self):
-        return f'$a\cdot b^x,\quad a={self.coefficients[0].__str__(pretty = True)}, \quad b={self.coefficients[1].__str__(pretty = True)}$'
+        a,b,c,d = self.coefficients
+        return f'$a\cdot b^(x-c)+d,\quad a={a.__str__(pretty = True)}, \quad b={b.__str__(pretty = True)}, \quad c={c.__str__(pretty = True)}, \quad d={d.__str__(pretty = True)}$'
 
 
 class pow_fit(_fit):
     def __init__(self, x, y, p0=[1, 1]):
         
         if len(p0) != 2:
             raise ValueError('You have to provide initial guesses for 2 parameters')
```

### Comparing `pyees-1.3.8/pyees/profileFit.py` & `pyees-1.3.9/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/profilePyees.py` & `pyees-1.3.9/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/prop.py` & `pyees-1.3.9/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/sheet.py` & `pyees-1.3.9/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/solve.py` & `pyees-1.3.9/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/stackOverflowODR.py` & `pyees-1.3.9/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/testFit.py` & `pyees-1.3.9/pyees/testFit.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,20 +144,20 @@
         self.assertAlmostEqual(F.r_squared, 1)
 
     def testExpFit(self):   
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100])
         y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
         f = exp_fit(x,y)
         
-        a,b  = f.coefficients
+        a,b,c,d  = f.coefficients
 
         self.assertEqual(b.unit, '1')
         self.assertEqual(a.unit, y.unit)
-        self.assertRelativeDifference(a.value, 1.0754076064, 5e-2)
-        self.assertRelativeDifference(b.value, np.e ** 0.0488105475, 1e-3)
+        self.assertRelativeDifference(a.value, 0.9875635849080608, 5e-2)
+        self.assertRelativeDifference(b.value, 1.0515901240689571, 1e-3)
         
         x = variable([20, 30, 40, 50, 60, 70, 80, 90, 100], 'C')
         y = variable([2.7331291071103,4.83637470698903,7.76023628649736,12.92164947233590,19.26005212361100,29.98037228450110,58.70407550133760,82.8915749115424,144.581793442337], 'kg/m3') 
 
         with self.assertRaises(Exception) as context:
             f = exp_fit(x,y)
         self.assertTrue('The variable "x" cannot have a unit' in str(context.exception))
```

### Comparing `pyees-1.3.8/pyees/testProp.py` & `pyees-1.3.9/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/testPyees.py` & `pyees-1.3.9/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/testSheet.py` & `pyees-1.3.9/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/testSolve.py` & `pyees-1.3.9/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/testUnit.py` & `pyees-1.3.9/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/testVariable.py` & `pyees-1.3.9/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/unit.py` & `pyees-1.3.9/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees/variable.py` & `pyees-1.3.9/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.8/pyees.egg-info/PKG-INFO` & `pyees-1.3.9/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.8
+Version: 1.3.9
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.8/setup.py` & `pyees-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.8',
+    version='1.3.9',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

