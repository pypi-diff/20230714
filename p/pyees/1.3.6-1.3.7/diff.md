# Comparing `tmp/pyees-1.3.6.tar.gz` & `tmp/pyees-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.6.tar", last modified: Fri Jun 30 12:09:06 2023, max compression
+gzip compressed data, was "pyees-1.3.7.tar", last modified: Fri Jul 14 08:17:33 2023, max compression
```

## Comparing `pyees-1.3.6.tar` & `pyees-1.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:09:06.717398 pyees-1.3.6/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-06-30 12:09:06.723383 pyees-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 12:09:06.518934 pyees-1.3.6/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.6/pyees/__init__.py
--rw-rw-rw-   0        0        0    13756 2023-06-30 12:08:37.000000 pyees-1.3.6/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.3.6/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10013 2023-06-30 11:34:55.000000 pyees-1.3.6/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.6/pyees/sheet.py
--rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.6/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.6/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-06-30 12:05:47.000000 pyees-1.3.6/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-06-30 11:31:13.000000 pyees-1.3.6/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.6/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.6/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.6/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.6/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.6/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.6/pyees/unit.py
--rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.6/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:09:06.691468 pyees-1.3.6/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-30 12:09:06.749313 pyees-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-06-30 12:08:56.000000 pyees-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:17:33.537316 pyees-1.3.7/
+-rw-rw-rw-   0        0        0     1085 2023-07-14 08:17:32.954907 pyees-1.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-14 08:17:33.542302 pyees-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 08:17:33.391713 pyees-1.3.7/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.7/pyees/__init__.py
+-rw-rw-rw-   0        0        0    13747 2023-07-13 16:45:15.000000 pyees-1.3.7/pyees/fit.py
+-rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.3.7/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.3.7/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.7/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.3.7/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2023-07-14 08:17:33.180291 pyees-1.3.7/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-06-30 12:05:47.000000 pyees-1.3.7/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.3.7/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.7/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.7/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.3.7/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.3.7/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83313 2023-07-13 19:18:16.000000 pyees-1.3.7/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.3.7/pyees/unit.py
+-rw-rw-rw-   0        0        0    34098 2023-07-13 19:38:36.000000 pyees-1.3.7/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:17:33.518366 pyees-1.3.7/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 08:17:32.000000 pyees-1.3.7/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-14 08:17:33.564242 pyees-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-14 08:17:22.000000 pyees-1.3.7/setup.py
```

### Comparing `pyees-1.3.6/LICENSE.txt` & `pyees-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/PKG-INFO` & `pyees-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.6
+Version: 1.3.7
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.6/README.md` & `pyees-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/fit.py` & `pyees-1.3.7/pyees/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,16 +342,16 @@
         units = []
         n = self.deg
         index = 0
         for i in range(n + 1):
             if self.terms[i]:
                 u = self.yUnit
                 if i != n:
-                    ui, _ = self.xUnit ** (n - i)
-                    u /= unit(ui)
+                    ui = self.xUnit ** (n - i)
+                    u /= ui
                 units.append(u)
                 index += 1
         return units
 
     def _func(self, B, x):
         out = 0
         n = self.deg
```

### Comparing `pyees-1.3.6/pyees/profilePyees.py` & `pyees-1.3.7/pyees/profilePyees.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,25 @@
     from variable import variable
 except ImportError:
     from pyees.variable import variable
     
 pr = cProfile.Profile()
 pr.enable()
 
-for _ in range(10000):
+for _ in range(10_000):
 
-    c = variable(4.182, 'J/kg-K', 130)
+    c = variable(4.182, 'J/kg-K', 0.130)
     rho = variable(1000, 'kg/m3', 0.01)
     t_in = variable(50, 'C', 1.2)
     t_out = variable([10, 15, 20, 25, 30, 35, 40], 'C', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
     v_dot = variable(300, 'L/min', 3)
     air_speed = variable([6.5, 6, 5.5, 5, 4.5, 4, 3.5], 'm/s', [0.1, 0.15, 0.12, 0.13, 0.9, 1.1, 1.0])
     q = c * rho * v_dot * (t_in - t_out)
     q.convert('kW')
 
-
 pr.disable()
 s = io.StringIO()
 ps = pstats.Stats(pr, stream=s).sort_stats('tottime')
 ps.print_stats()
 
 with open('profile.txt', 'w+') as f:
     f.write(s.getvalue())
```

### Comparing `pyees-1.3.6/pyees/prop.py` & `pyees-1.3.7/pyees/prop.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 
 def isAllArgumentsUsed(arguments: dict):
     if (len(arguments.keys()) > 0):
         raise ValueError(f'The inputs {list(arguments.keys())} are not appropriate for this fluid')
 
 def findArgument(arguments : dict, parameterName, unitStr, raiseError = True):
 
-    desiredSIBaseUnit = unit(unitStr)._SIBaseUnit
+    desiredSIBaseUnit = unit(unitStr).unitStrSI
     
     parameter = None
     if  parameterName in arguments.keys():
         parameter = arguments[parameterName]
         del arguments[parameterName]
     else:
         if raiseError:
             raise ValueError(f'Could not find an arugment matching that of a {parameterName}')
     if not parameter is None:
-        if parameter._unitObject._SIBaseUnit != desiredSIBaseUnit:
+        if parameter._unitObject.unitStrSI != desiredSIBaseUnit:
             raise ValueError(f'The input {parameterName} did not have to correct unit of {unitStr}')
 
     return arguments, parameter
 
 def differentialsBrine(fluid : Fluid, fluidName,  property, C, parameters):
 
     vars, grads = differentials(fluid, property, parameters)
@@ -48,26 +48,23 @@
     y1 = getattr(Fluid(fluidName,C.value*(1 + dx)).with_state(*fluid._inputs), property)
     y2 = getattr(Fluid(fluidName,C.value*(1 - dx)).with_state(*fluid._inputs), property)
 
     grads.append((y2-y1) / (2*dx * C.value))
     vars.append(C)
     return vars, grads
 
-
 def differentials(fluid : Fluid, property : str, parameters):
     vars = []
     indexes = []
     for i, param in enumerate(parameters):
         if param.uncert != 0:
             indexes.append(i)
             vars.append(param)
     
-    
     inputs = list(fluid._inputs)
-
     
     grads = []
     for i in indexes:
         
         i0 = inputs[i]
         i1 = Input(i0.coolprop_key, i0.value * (1-dx))
         i2 = Input(i0.coolprop_key, i0.value * (1+dx))
@@ -82,15 +79,14 @@
         
         inputs[i] = i0
         fluid.update(*inputs)
         
         grads.append((y2-y1) / (2*dx*i0.value))
     
     return vars, grads
-    
 
 def outputFromParameters(scalarMethod, property, params):
     
     ## determine which of the parameters that are arrayVariables
     isArrayVariable = [hasattr(param, '__len__') for param in params]
     
     ## return the scalarmethod if all parameters are scalarvariables
@@ -311,15 +307,15 @@
     'MEG': propMEG,
     'air': propHumidAir
 }
 
 
 if __name__ == "__main__":
 
-    T = variable([20,25,30], 'C', [0.1, 0.2, 0.15])
-    P = variable([1, 1.1, 1.2], 'bar', [0.03, 0.04, 0.025])
+    # T = variable([20,25,30], 'C', [0.1, 0.2, 0.15])
+    # P = variable([1 * 1e5, 1.1 * 1e5, 1.2 * 1e5], 'Pa', [0.03 * 1e5, 0.04 * 1e5, 0.025 * 1e5])
     
-    rho = prop('density', 'water', T = T, P = P)
-    for elem in rho:
-        for key, item in elem.dependsOn.items():
-            print(key, item[1])
+    # rho = prop('density', 'water', T = T, P = P)
+    # print(rho)
+    P = variable(1, 'bar')
+    print(P._unitObject._converterToSI.scale)
```

### Comparing `pyees-1.3.6/pyees/sheet.py` & `pyees-1.3.7/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/solve.py` & `pyees-1.3.7/pyees/solve.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     for o in out:
         if (len(o) != 2):
             raise ValueError('Each equation has to be a list of 2 elements')
         for bound in o:
             if not isinstance(bound, scalarVariable):
                 raise ValueError('Each side of each equation has to be a variable')        
         ## test if the units match
-        if (o[0]._unitObject._SIBaseUnit != o[1]._unitObject._SIBaseUnit):
+        if (o[0]._unitObject.unitDictSI != o[1]._unitObject.unitDictSI):
                 raise ValueError('The units of the equations does not match')
         doesUnitsOfEquationsMatch.append(o[0].unit == o[1].unit)
     
     
     ## determine the number of variables and if the variables are arrayVariables
     nVariables = 0
     for xi in x:
@@ -97,15 +97,15 @@
                 
                 ## check that all elements of the bounds are variables
                 for bound in o:
                     if not isinstance(bound, scalarVariable):
                         raise ValueError('Each side of the bounds has to be a variable')         
                 
                 ## check the units bounds
-                if (o[0]._unitObject._SIBaseUnit != o[1]._unitObject._SIBaseUnit or o[1]._unitObject._SIBaseUnit != o[2]._unitObject._SIBaseUnit):
+                if (o[0]._unitObject.unitDictSI != o[1]._unitObject.unitDictSI or o[1]._unitObject.unitDictSI != o[2]._unitObject.unitDictSI):
                     raise ValueError('The units of the bounds does not match')
                 
                 ## chekc that all elements in the bounds have the same length
                 try:
                     for _,_,_ in zip(o[0], o[1], o[2], strict = True): pass
                 except ValueError:
                     raise ValueError('Each element of the bounds has to have the same length')
@@ -131,15 +131,15 @@
             for i, bound in enumerate(bounds):
                 
                 for elem in bound:
                     ## check that the elements are variables
                     if not isinstance(elem, scalarVariable):
                         raise ValueError('All bounds has to be variables')
                      ## check the units bounds
-                    if (elem._unitObject._SIBaseUnit != x[i]._unitObject._SIBaseUnit):
+                    if (elem._unitObject.unitDictSI != x[i]._unitObject.unitDictSI):
                         raise ValueError('The units of the bounds does not match with the corresponding variable')
                     
                     ## convert the bounds to the units of the corresponding variable
                     elem.convert(x[i].unit)
                 
                 ## collect the bounds in bbounds
                 try:
@@ -156,15 +156,15 @@
     scales = np.ones(nVariables)
     if nVariables != 1:
         out = ffunc(*x)
         currentIndex = 0
         for i,o in enumerate(out):
             if not doesUnitsOfEquationsMatch[i]:
                 for elem in o:
-                    elem.convert(elem._unitObject._SIBaseUnit) 
+                    elem.convert(elem._unitObject.unitStrSI) 
             scales[i] = 1/(o[0].value - o[1].value)**2
     
     
     ## method to keep the variables within the bounda
     ## the method will be given a single input during the minimzation. 
     ## Therefore a single input argument is defined which is never used
     def keepVariablesFeasible(_ = None):
@@ -188,15 +188,15 @@
         ## evaluate the function
         out = ffunc(*x)
         
         ## convert all equations to the SI unit system, if each side of the units are not identical
         for b,o in zip(doesUnitsOfEquationsMatch, out):
             if not b:
                 for elem in o:
-                    elem.convert(elem._unitObject._SIBaseUnit)
+                    elem.convert(elem._unitObject.unitStrSI)
 
         return sum([(e[0].value - e[1].value)**2 * s for e,s in zip(out, scales)])
 
 
     ## move the initial guess in to the feasible area if the bounds are callable
     if callable(bounds): keepVariablesFeasible()
     
@@ -224,15 +224,15 @@
     if callable(bounds): keepVariablesFeasible()
 
 
     ## loop over all equations and create a list of the residuals
     residuals, J = [], np.zeros([nVariables,nVariables])
     for i, equation in enumerate(_func(*x)):
         res = equation[0] - equation[1]
-        res.convert(res._unitObject._SIBaseUnit)
+        res.convert(res._unitObject.unitStrSI)
         for bound in res:
             residuals.append(bound)
 
 
     ## create the jacobian matrix from the residual
     for i, res in enumerate(residuals):
         ## loop over the variables
```

### Comparing `pyees-1.3.6/pyees/stackOverflowODR.py` & `pyees-1.3.7/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/testFit.py` & `pyees-1.3.7/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/testProp.py` & `pyees-1.3.7/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/testPyees.py` & `pyees-1.3.7/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/testSheet.py` & `pyees-1.3.7/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.6/pyees/testSolve.py` & `pyees-1.3.7/pyees/testSolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,16 +169,14 @@
         x0 = [variable(1,''), variable(1,'')]
         x,y = solve(func, x0, tol = solveTol)
                 
         self.assertRelativeDifference(x.value, correctX.value, tol)
         self.assertRelativeDifference(y.value, correctY.value, tol)
         self.assertRelativeDifference(x.uncert, correctX.uncert, tol)
         self.assertRelativeDifference(y.uncert, correctY.uncert, tol)
-
-
    
     def testSolveOneNonlinearEquationWithBounds1(self):
         lbs = [variable(-10,'L/min'), variable(10, 'L/min')]
         ubs = [variable(5,'L/min'), variable(100, 'L/min')]
         
         
         for lb in lbs:
@@ -301,15 +299,14 @@
 
         bounds = [variable(0.06, 'm3/h'), variable(1.667,'L/s')]
             
         x = solve(func, variable(100,'L/min'), bounds = bounds, tol = solveTol)
         
         self.assertRelativeDifference(x.value, correct.value, tol)
     
-    
     def testSolveOneNonlinearEquationWithBoundsUsingDifferentUnits2(self):
                 
         a = variable(23.7, 'mbar-min2/L2', 0.1)
         b = variable(943, 'mbar', 12.5)
         correct = (b / a)**(1/2)
         
         def func(x):
@@ -342,15 +339,14 @@
         x0 = variable(20, 'C')
         t_out = solve(func, x0, tol = solveTol)
         
         self.assertRelativeDifference(t_out.value, 54.36480373585032900, tol)
         self.assertEqual(t_out.unit, 'C')
         self.assertRelativeDifference(t_out.uncert, 1.217157659256291610, tol)
      
-
     def testSolveOneNonlinearEquationWithVectors(self):
         a = variable([23.7, 12.3], '', [0.1, 0.05])
         b = variable([943, 793], '', [12.5, 9.4])
         
         def func(x):
             return [a * x**2, b]
         
@@ -399,15 +395,14 @@
         for c, l in zip(correct, lower):
             if c < l:
                 c._value = l.value
         
         for i in range(len(x)):
             self.assertRelativeDifference(x[i].value, correct[i].value, tol)
 
-
     def testCallableBoundInputs(self):
         a = variable([23.7, 12.3], '', [0.1, 0.05])
         b = variable([943, 793], '', [12.5, 9.4])
         
         def func(x):
             return [a * x**2, b]
```

### Comparing `pyees-1.3.6/pyees/testUnit.py` & `pyees-1.3.7/pyees/testUnit.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,118 +4,171 @@
 except ImportError:
     from pyees.unit import unit, addNewUnit
 
 class test(unittest.TestCase):
 
     def testPower(self):
         A = unit('L-kg/min')
-        with self.assertRaises(Exception) as context:
-            A**1.5
-        self.assertEqual('The power has to be an integer', str(context.exception))
-        a, _ = A**2
-        self.assertEqual(str(a), 'L2-kg2/min2')
+        a = A**2
+        self.assertTrue(a == unit('L2-kg2/min2'))
 
         B = unit('m/s2')
-        b, _ = B**0
-        self.assertEqual(str(b), '1')
+        b = B**0
+        self.assertTrue(b == unit('1'))
 
         C = unit('L2/h2')
-        c, _ = C**0.5
-        self.assertEqual(str(c), 'L/h')
+        c = C**0.5
+        self.assertTrue(c == unit('L/h'))
 
     def testMultiply(self):
         a = unit('L/min')
         b = unit('kg-m/L')
         """ (L/min) * (kg-m/L)
             L-kg-m/min-L
             kg-m/min    """
         c = a * b
-        self.assertTrue(unit(c)._assertEqual('kg-m/min'))
+        self.assertTrue(c == unit('kg-m/min'))
 
         a = unit('L/min')
         b = unit('L/min')
         c = a * b
-        self.assertEqual(str(c), 'L2/min2')
+        self.assertTrue(c == unit('L2/min2'))
 
         a = unit('km')
         b = unit('1/m')
         c = a * b
-        self.assertEqual(str(c), 'km/m')
+        self.assertTrue(c == unit('km/m'))
+        
+        a = unit('m/N')
+        b = unit('N/cm')
+        c = a * b
+        self.assertTrue(c == unit('m/cm'))
+        
 
     def testDivide(self):
 
         a = unit('L/min')
         b = unit('L/min')
         c = a / b
-        self.assertEqual(str(c), '1')
+        self.assertTrue(c == unit('1'))
 
         a = unit('L/min')
         b = unit('kg-m/L')
-        """ L/min / (kg-m/L)
-            L/min * L/kg-m
+        """ (L/min) / (kg-m/L)
+            (L/min) * (L/kg-m)
             L2 / min-kg-m """
         c = a / b
-
-        self.assertTrue(unit('L2/min-kg-m')._assertEqual(unit(c)))
+        self.assertTrue(c == unit('L2/min-kg-m'))
 
         A = unit('m')
         B = unit('cm')
         c = A / B
-        self.assertEqual(c, 'm/cm')
+        self.assertTrue(c == unit('m/cm'))
+    
+        
 
     def testAdd(self):
         a = unit('L/min')
         b = unit('kg-m/L')
 
         with self.assertRaises(Exception) as context:
             a + b
         self.assertTrue('You tried to add a variable in [L/min] to a variable in [kg-m/L], but the units do not have the same SI base unit' in str(context.exception))
         
         a = unit('L/min')
         b = unit('L/min')
-        _,cUnit,_,_,_ = a + b
-        self.assertEqual(cUnit, 'L/min')
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('L/min'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
 
         a = unit('m-K/L-bar')
         b = unit('K-m/bar-L')
-        _,cUnit,_,_,_ = a + b
-        self.assertTrue(unit._assertEqualStatic(cUnit, 'DELTAK-m/bar-L'))
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('DELTAK-m/bar-L'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
         
         a = unit('J/kg-DELTAK')
         b = unit('J/kg-DELTAK')
-        _,cUnit,_,_,_ = a + b
-        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/kg-DELTAK'))
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('J/kg-DELTAK'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
         
         a = unit('J/g-DELTAK')
         b = unit('J/kg-DELTAK')
-        _,cUnit,_,_,_ = a + b
-        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/g-DELTAK'))
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('J/g-DELTAK'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
+        
+        a = unit('dB')
+        b = unit('dB')
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('dB'))
+        self.assertTrue(outputUnit.isLogarithmicUnit())
+        
+        a = unit('mB')
+        b = unit('dB')
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('B'))
+        self.assertTrue(outputUnit.isLogarithmicUnit())
+        
+        a = unit('L/min')
+        b = unit('m3/h')
+        outputUnit = a + b
+        self.assertTrue(outputUnit == unit('m3/s'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
         
     def testSub(self):
         a = unit('L/min')
         b = unit('kg-m/L')
-        
+
         with self.assertRaises(Exception) as context:
-            a-b
+            a - b
         self.assertTrue('You tried to subtract a variable in [kg-m/L] from a variable in [L/min], but the units do not have the same SI base unit' in str(context.exception))
         
         a = unit('L/min')
         b = unit('L/min')
-        _,cUnit,_,_,_ = a - b
-        self.assertEqual(str(cUnit), 'L/min')
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('L/min'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
+
+        a = unit('m-K/L-bar')
+        b = unit('K-m/bar-L')
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('DELTAK-m/bar-L'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
         
         a = unit('J/kg-DELTAK')
         b = unit('J/kg-DELTAK')
-        _,cUnit,_,_,_ = a - b
-        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/kg-DELTAK'))
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('J/kg-DELTAK'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
         
         a = unit('J/g-DELTAK')
         b = unit('J/kg-DELTAK')
-        _,cUnit,_,_,_ = a - b
-        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/g-DELTAK'))
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('J/g-DELTAK'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
+        
+        a = unit('dB')
+        b = unit('dB')
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('dB'))
+        self.assertTrue(outputUnit.isLogarithmicUnit())
+        
+        a = unit('mB')
+        b = unit('dB')
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('B'))
+        self.assertTrue(outputUnit.isLogarithmicUnit())
+        
+        a = unit('L/min')
+        b = unit('m3/h')
+        outputUnit = a - b
+        self.assertTrue(outputUnit == unit('m3/s'))
+        self.assertFalse(outputUnit.isLogarithmicUnit())
 
     def testConvert(self):
         a = unit('L/min')
         converter = a.getConverter('m3/h')
         self.assertAlmostEqual(converter.convert(1), 0.06)
 
         a = unit('K')
@@ -142,21 +195,19 @@
         converter = a.getConverter('m2')
         self.assertAlmostEqual(converter.convert(1), 1/1000 * 1/1000)
 
 
         a = unit('A')
         b = unit('V')
         c = a * b
-        c = unit(c)
         converter = c.getConverter('W')
         
         a = unit('A')
         b = unit('ohm')
         c = a * b
-        c = unit(c)
         converter = c.getConverter('V')
         
         self.assertEqual(converter.convert(1, useOffset=True), 1)
 
         with self.assertRaises(Exception) as context:
             a = unit('mu')
         self.assertEqual('''The unit (mu) was not found. Therefore it was interpreted as a prefix and a unit. The prefix was identified as "mu" and the unit was identified as "1". However, the unit "1" cannot have a prefix''', str(context.exception))
@@ -173,46 +224,45 @@
         with self.assertRaises(Exception) as context:
             converter = a.getConverter('m')
         self.assertEqual('You tried to convert from L/min to m. But these do not have the same base units', str(context.exception))
 
     def testInput(self):
 
         a = unit(None)
-        self.assertEqual(str(a), '1')
+        self.assertTrue(a == unit('1'))
         
         a = unit('m / s')
-        self.assertEqual(str(a), 'm/s')
+        self.assertTrue(a == unit('m/s'))
 
         with self.assertRaises(Exception) as context:
             a = unit('m!/s')
-        self.assertEqual('The character ! is not used within the unitsystem', str(context.exception))
+        self.assertTrue('The character ! is not used within the unitsystem', str(context.exception))
 
         with self.assertRaises(Exception) as context:
             a = unit('m/s/bar')
-        self.assertEqual('A unit can only have a single slash (/)', str(context.exception))
+        self.assertTrue('A unit can only have a single slash (/)', str(context.exception))
 
-        self.assertEqual(str(unit(' ')), '1')
-        self.assertEqual(str(unit('-')), '1')
-        self.assertEqual(str(unit('')), '1')
-        self.assertEqual(str(unit('--')), '1')
-        self.assertEqual(str(unit('- -')), '1')
-        
-        self.assertEqual(str(unit('()')), '1')
-        self.assertEqual(str(unit('( )')), '1')
-        self.assertEqual(str(unit('(  )')), '1')  
-        self.assertEqual(str(unit('(-)')), '1')
-        self.assertEqual(str(unit('(--)')), '1')
-        self.assertEqual(str(unit('(- -)')), '1')
-        self.assertEqual(str(unit('( -)')), '1')
-        self.assertEqual(str(unit('( - (- ))')), '1')
-        
-        
-        self.assertEqual(str(unit('(m/s2)2/Hz')), 'm2/s4-Hz')
-        self.assertEqual(str(unit('(m1/s2)2/Hz')), 'm2/s4-Hz')
-        self.assertEqual(str(unit('(m1/s2)1/Hz')), 'm/s2-Hz')
+        self.assertTrue(unit(' ') == unit('1'))
+        self.assertTrue(unit('-') == unit('1'))
+        self.assertTrue(unit('') == unit('1'))
+        self.assertTrue(unit('--') == unit('1'))
+        self.assertTrue(unit('- -') == unit('1'))
+        
+        self.assertTrue(unit('()') == unit('1'))
+        self.assertTrue(unit('( )') == unit('1'))
+        self.assertTrue(unit('(  )') == unit('1'))  
+        self.assertTrue(unit('(-)') == unit('1'))
+        self.assertTrue(unit('(--)') == unit('1'))
+        self.assertTrue(unit('(- -)') == unit('1'))
+        self.assertTrue(unit('( -)') == unit('1'))
+        self.assertTrue(unit('( - (- ))') == unit('1'))
+        
+        self.assertTrue(unit('(m/s2)2/Hz') == unit('m2/s4-Hz'))
+        self.assertTrue(unit('(m1/s2)2/Hz') == unit('m2/s4-Hz'))
+        self.assertTrue(unit('(m1/s2)1/Hz') == unit('m/s2-Hz'))
 
     def testAddNewUnit(self):
         addNewUnit('gnA', 9.81, 'm/s2')
         converter = unit('gnA').getConverter('m/s2')
         self.assertEqual(converter.convert(1), 9.81)
         
         addNewUnit('gnB', 9.81, 'm/s2', 0)
```

### Comparing `pyees-1.3.6/pyees/testVariable.py` & `pyees-1.3.7/pyees/testVariable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import unittest
 import numpy as np
-from random import uniform
 try:
     from variable import variable
+    from unit import unit
 except ImportError:
     from pyees.variable import variable
-
+    from pyees.unit import unit
+    
 class test(unittest.TestCase): 
 
     def testSingleNumber(self):
         A = variable(1.3, 'm')
         B = variable(2.0, 'm', 0.01)
         C = variable([1.0, 1.3], 'L/min', np.array([20, 30]))
         D = variable(np.array([11, 1111]), 'L/min', [2.1, 3.9])
@@ -90,15 +91,14 @@
 
         A = variable(7, '%', 0.1)
         B = 1 + A
         self.assertAlmostEqual(B.value, 8)
         self.assertEqual(B.unit, '%')
         self.assertEqual(B.uncert, 0.1)
 
-
     def test_sub(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'L/min', uncert=53.9)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'L/min', uncert=[53.9, 24.75, 6.4])
 
         C = A - B
@@ -230,86 +230,93 @@
         
         a = variable(10, 'C', 1.2)
         b = variable(100, 'muC', 3.9)
         c = a - b
         self.assertAlmostEqual(c.value, 10 - 100 * 1e-6)
         self.assertEqual(c.unit, 'DELTAC')
         self.assertEqual(c.uncert, np.sqrt((1 * 1.2)**2 + (1 * 3.9*1e-6)**2))
+        
+        a = variable(100, 'muC', 3.9)
+        b = variable(10, 'C', 1.2)
+        c = a - b
+        self.assertAlmostEqual(c.value, -10 + 100 * 1e-6)
+        self.assertEqual(c.unit, 'DELTAC')
+        self.assertEqual(c.uncert, np.sqrt((1 * 1.2)**2 + (1 * 3.9*1e-6)**2))
 
     def test_multiply(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'm', uncert=53.9)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'm', uncert=[53.9, 24.75, 6.4])
 
         C = A * B
 
         self.assertAlmostEqual(C.value, 12.3 * 745.1)
-        self.assertTrue(C._unitObject._assertEqual('L-m/min'))
+        self.assertTrue(C._unitObject == unit('L-m/min'))
         self.assertAlmostEqual(C.uncert, np.sqrt((745.1 * 2.6)**2 + (12.3 * 53.9)**2))
 
         C_vec = A_vec * B_vec
         np.testing.assert_array_equal(C_vec.value, np.array([12.3 * 745.1, 54.3 * 496.13, 91.3 * 120.54]))
-        self.assertTrue(C._unitObject._assertEqual('L-m/min'))
+        self.assertTrue(C._unitObject == unit('L-m/min'))
         np.testing.assert_array_almost_equal(
             C_vec.uncert,
             np.array([
                 np.sqrt((745.1 * 2.6)**2 + (12.3 * 53.9)**2),
                 np.sqrt((496.13 * 5.4)**2 + (54.3 * 24.75)**2),
                 np.sqrt((120.54 * 10.56)**2 + (91.3 * 6.4)**2),
             ]))
 
         C_vec.convert('m3-km / s')
         np.testing.assert_array_equal(C_vec.value, np.array([12.3 * 745.1, 54.3 * 496.13, 91.3 * 120.54]) / 1000 / 1000 / 60)
-        self.assertEqual(C_vec.unit, 'm3-km/s')
+        self.assertTrue(C_vec._unitObject == unit('m3-km/s'))
         np.testing.assert_almost_equal(
             C_vec.uncert,
             np.array([
                 np.sqrt((745.1 / 1000 * 2.6 / 1000 / 60)**2 + (12.3 / 1000 / 60 * 53.9 / 1000)**2),
                 np.sqrt((496.13 / 1000 * 5.4 / 1000 / 60)**2 + (54.3 / 1000 / 60 * 24.75 / 1000)**2),
                 np.sqrt((120.54 / 1000 * 10.56 / 1000 / 60)**2 + (91.3 / 1000 / 60 * 6.4 / 1000)**2),
             ]), decimal=7)
 
         a = variable(1.2, 'm/N', 0.15)
         b = variable(7.43, 'N/cm', 2.5)
         c = a * b
         self.assertAlmostEqual(c.value, 891.6)
-        self.assertEqual(c.unit, '1')
+        self.assertTrue(c._unitObject == unit('1'))
         self.assertAlmostEqual(c.uncert, 320.032970958)
 
     def test_divide(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'm', uncert=53.9)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'm', uncert=[53.9, 24.75, 6.4])
 
         C = A / B
         self.assertAlmostEqual(C.value, 12.3 / 745.1)
-        self.assertTrue(C._unitObject._assertEqual('L/min-m'))
+        self.assertTrue(C._unitObject == unit('L/min-m'))
         self.assertAlmostEqual(C.uncert, np.sqrt((1 / 745.1 * 2.6)**2 + (12.3 / (745.1**2) * 53.9)**2))
 
         C.convert('m3/h-mm')
         self.assertAlmostEqual(C.value, 12.3 / 745.1 / 1000 * 60 / 1000)
-        self.assertEqual(C.unit, 'm3/h-mm')
+        self.assertTrue(C._unitObject == unit('m3/h-mm'))
         self.assertAlmostEqual(C.uncert, np.sqrt((1 / (745.1 * 1000) * 2.6 / 1000 * 60)**2 + (12.3 / ((745.1)**2) * 53.9 / 1000 * 60 / 1000)**2))
 
         C_vec = A_vec / B_vec
         np.testing.assert_array_equal(C_vec.value, np.array([12.3 / 745.1, 54.3 / 496.13, 91.3 / 120.54]))
-        self.assertTrue(C_vec._unitObject._assertEqual('L/min-m'))
+        self.assertTrue(C_vec._unitObject == unit('L/min-m'))
         np.testing.assert_array_almost_equal(
             C_vec.uncert,
             np.array([
                 np.sqrt((1 / 745.1 * 2.6)**2 + (12.3 / (745.1)**2 * 53.9)**2),
                 np.sqrt((1 / 496.13 * 5.4)**2 + (54.3 / (496.13)**2 * 24.75)**2),
                 np.sqrt((1 / 120.54 * 10.56)**2 + (91.3 / (120.54)**2 * 6.4)**2),
             ]))
 
         C_vec.convert('m3 / h -mm')
         np.testing.assert_almost_equal(C_vec.value, np.array([12.3 / 745.1, 54.3 / 496.13, 91.3 / 120.54]) / 1000 * 60 / 1000)
-        self.assertEqual(C_vec.unit, 'm3/h-mm')
+        self.assertTrue(C_vec._unitObject == unit('m3/h-mm')) 
         np.testing.assert_almost_equal(
             C_vec.uncert,
             np.array([
                 np.sqrt((1 / 745.1 * 2.6 / 1000 * 60 / 1000)**2 + (12.3 / (745.1)**2 * 53.9 / 1000 * 60 / 1000)**2),
                 np.sqrt((1 / 496.13 * 5.4 / 1000 * 60 / 1000)**2 + (54.3 / (496.13)**2 * 24.75 / 1000 * 60 / 1000)**2),
                 np.sqrt((1 / 120.54 * 10.56 / 1000 * 60 / 1000)**2 + (91.3 / (120.54)**2 * 6.4 / 1000 * 60 / 1000)**2),
             ]))
@@ -698,15 +705,15 @@
 
     def testMultiEqual(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'm', uncert=53.9)
 
         A *= B
         self.assertAlmostEqual(A.value, 12.3 * 745.1)
-        self.assertTrue(A._unitObject._assertEqual('L-m/min'))
+        self.assertTrue(A._unitObject, unit('L-m/min'))
         self.assertAlmostEqual(A.uncert, np.sqrt((745.1 * 2.6)**2 + (12.3 * 53.9)**2))
 
         A = variable(12.3, 'L/min', uncert=2.6)
         A *= 2
         self.assertAlmostEqual(A.value, 12.3 * 2)
         self.assertEqual(A.unit, 'L/min')
         self.assertAlmostEqual(A.uncert, np.sqrt((2 * 2.6)**2))
@@ -719,15 +726,15 @@
         self.assertAlmostEqual(B.uncert, np.sqrt((2 * 2.6)**2))
 
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'm', uncert=[53.9, 24.75, 6.4])
 
         A_vec *= B_vec
         np.testing.assert_array_almost_equal(A_vec.value, np.array([12.3 * 745.1, 54.3 * 496.13, 91.3 * 120.54]))
-        self.assertTrue(A_vec._unitObject._assertEqual('L-m/min'))
+        self.assertTrue(A_vec._unitObject, unit('L-m/min'))
         np.testing.assert_array_almost_equal(
             A_vec.uncert,
             np.array([
                 np.sqrt((745.1 * 2.6)**2 + (12.3 * 53.9)**2),
                 np.sqrt((496.13 * 5.4)**2 + (54.3 * 24.75)**2),
                 np.sqrt((120.54 * 10.56)**2 + (91.3 * 6.4)**2),
             ]))
@@ -747,49 +754,49 @@
 
     def testDivEqual(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'm', uncert=53.9)
 
         A /= B
         self.assertAlmostEqual(A.value, 12.3 / 745.1)
-        self.assertTrue(A._unitObject._assertEqual('L/min-m'))
+        self.assertTrue(A._unitObject == unit('L/min-m'))
         self.assertAlmostEqual(A.uncert, np.sqrt((1 / 745.1 * 2.6)**2 + (12.3 / (745.1**2) * 53.9)**2))
 
         A = variable(12.3, 'L/min', uncert=2.6)
         A /= 2
         self.assertAlmostEqual(A.value, 12.3 / 2)
-        self.assertEqual(A.unit, 'L/min')
+        self.assertTrue(A._unitObject == unit('L/min'))
         self.assertAlmostEqual(A.uncert, np.sqrt((1 / 2 * 2.6)**2))
 
         A = variable(12.3, 'L/min', uncert=2.6)
         B = 2
         B /= A
         self.assertAlmostEqual(B.value, 2 / 12.3)
-        self.assertEqual(B.unit, 'min/L')
+        self.assertTrue(B._unitObject == unit('min/L'))
         self.assertAlmostEqual(B.uncert, np.sqrt((2 / (12.3**2) * 2.6)**2))
 
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'm', uncert=[53.9, 24.75, 6.4])
 
         A_vec /= B_vec
         np.testing.assert_array_almost_equal(A_vec.value, np.array([12.3 / 745.1, 54.3 / 496.13, 91.3 / 120.54]))
-        self.assertTrue(A_vec._unitObject._assertEqual('L/min-m'))
+        self.assertTrue(A_vec._unitObject == unit('L/min-m'))
         np.testing.assert_array_almost_equal(
             A_vec.uncert,
             np.array([
                 np.sqrt((1 / 745.1 * 2.6)**2 + (12.3 / (745.1**2) * 53.9)**2),
                 np.sqrt((1 / 496.13 * 5.4)**2 + (54.3 / (496.13**2) * 24.75)**2),
                 np.sqrt((1 / 120.54 * 10.56)**2 + (91.3 / (120.54**2) * 6.4)**2),
             ]))
 
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         A = variable(12.3, 'L/min', uncert=2.6)
         A_vec /= A
         np.testing.assert_array_almost_equal(A_vec.value, np.array([12.3 / 12.3, 54.3 / 12.3, 91.3 / 12.3]))
-        self.assertEqual(A_vec.unit, '1')
+        self.assertTrue(A_vec._unitObject, unit('1'))
         np.testing.assert_array_almost_equal(
             A_vec.uncert,
             np.array([
                 np.sqrt((1 / 12.3 * 2.6)**2 + (12.3 / (12.3**2) * 2.6)**2),
                 np.sqrt((1 / 12.3 * 5.4)**2 + (54.3 / (12.3**2) * 2.6)**2),
                 np.sqrt((1 / 12.3 * 10.56)**2 + (91.3 / (12.3**2) * 2.6)**2),
             ]))
@@ -862,14 +869,15 @@
         A = variable(123456789 * 10**(-14), 'm', nDigits=5)
         self.assertEqual(str(A), '1.2346e-06 [m]')
 
         A = variable(123456789 * 10**(-16), 'm', nDigits=3)
         self.assertEqual(str(A), '1.23e-08 [m]')
 
     def testRoot(self):
+        from random import uniform
         A = variable(10, 'L2/min2')
         a = np.sqrt(A)
         self.assertEqual(a.value, np.sqrt(10))
         self.assertEqual(a.unit, 'L/min')
 
         a = A**(1 / 2)
         self.assertEqual(a.value, 10**(1 / 2))
@@ -929,16 +937,14 @@
         self.assertEqual(str(A), '0.05 +/- 0.07 [L/min]')
 
         A = variable(0.0543, 'L/min', 0.7)
         self.assertEqual(str(A), '0.1 +/- 0.7 [L/min]')
         
         A = variable(0.9, 'L/min', 3)
         self.assertEqual(str(A), '1 +/- 3 [L/min]')
-        
-        
 
     def testUnitless(self):
         with self.assertRaises(Exception) as context:
             A = variable(10, 'P', 1)
         self.assertTrue('''The unit (P) was not found. Therefore it was interpreted as a prefix and a unit. However a combination of prefix and unit which matches P was not found''' in str(context.exception))
 
         A = variable(10, '1', 1)
@@ -1194,20 +1200,20 @@
         self.assertEqual(b.unit, 'L2/min2')
         self.assertAlmostEqual(b.uncert, np.sqrt((1.5 * 4 * 200)**2))
 
         b /= 23.8
         self.assertAlmostEqual(b.value, 3361.3445378151260504201680672269)
         self.assertEqual(b.unit, 'L2/min2')
         self.assertAlmostEqual(b.uncert, np.sqrt((1.5 * 0.16806722689075630252100840336134 * 200)**2))
-
+       
         b *= np.sin(a * variable(1, 'rad-min/L'))
         self.assertAlmostEqual(b.value, -2935.453099878973383976532508069948132551783965504369163751)
         self.assertEqual(b.unit, 'L2/min2')
         self.assertAlmostEqual(b.uncert, np.sqrt((1.5 * 2 * 200 * (2 * np.sin(200) + 200 * np.cos(200)) / 23.8)**2))
-
+                
         a /= variable(100, 'L/min')
         a.convert('')
         b /= np.exp(a)
         self.assertAlmostEqual(b.value, -397.2703766999135885608809478456258749790006977070134430245)
         self.assertEqual(b.unit, 'L2/min2')
         self.assertAlmostEqual(b.uncert, np.sqrt((1.5 * 2 * 200 * np.exp(-200 / 100) * ((2 * 100 - 200) * np.sin(200) + 100 * 200 * np.cos(200)) / (23.8 * 100))**2))
 
@@ -1249,41 +1255,41 @@
 
     def testCovariance(self):
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
         a.addCovariance(b, 23, 'L-Pa/min')
         c = a * b
         self.assertEqual(c.value, 123 * 93)
-        self.assertTrue(c._unitObject._assertEqual('L-Pa/min'))
+        self.assertTrue(c._unitObject ==unit('L-Pa/min'))
         self.assertAlmostEqual(c.uncert, np.sqrt((123 * 1.2)**2 + (93 * 9.7)**2 + 2 * 93 * 123 * 23))
 
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
         a.addCovariance(b, 23, 'L-Pa/min')
         a.convert('m3/s')
         c = a * b
         self.assertEqual(c.value, 123 * 93 / 1000 / 60)
-        self.assertTrue(c._unitObject._assertEqual('m3-Pa/s'))
+        self.assertTrue(c._unitObject ==unit('m3-Pa/s'))
         self.assertEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23 / 1000 / 60))
         
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
         a.addCovariance(b, 23, 'm3-Pa/s')
         a.convert('m3/s')
         c = a * b
         self.assertEqual(c.value, 123 * 93 / 1000 / 60)
-        self.assertTrue(c._unitObject._assertEqual('m3-Pa/s'))
-        self.assertEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23))
+        self.assertTrue(c._unitObject ==unit('m3-Pa/s'))
+        self.assertAlmostEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23))
         
         a = variable([1, 2, 3], 'L/min', [0.1, 0.2 ,0.3])
         b = variable([93, 97, 102], 'Pa', [1.2, 2.4, 4.7])
         a.addCovariance(b, [2, 3, 4], 'L-Pa/min')
         c = a * b
         np.testing.assert_equal(c.value, [1*93, 2*97, 3*102])
-        self.assertTrue(c._unitObject._assertEqual('L-Pa/min'))
+        self.assertTrue(c._unitObject ==unit('L-Pa/min'))
         dcda = np.array([93, 97, 102], dtype = float)
         dcdb = np.array([1, 2, 3], dtype = float)
         ua = np.array([0.1, 0.2, 0.3], dtype = float)
         ub = np.array([1.2, 2.4, 4.7], dtype = float)
         uab = np.array([2, 3, 4], dtype = float)
 
         uc = np.sqrt((dcda * ua)**2 + (dcdb * ub)**2 + 2 * dcda * dcdb * uab)
@@ -1299,92 +1305,86 @@
         self.assertEqual(c.uncert,  np.sqrt((1 * 1000 * 0.1 * 1000*1000)**2 + (1 * 1000*1000 * 0.1 * 1000)**2))
         
         diameter = variable(40, 'cm', 0.2)
         area = np.pi / 4 * diameter ** 2
         area.convert('m2')
         self.assertEqual(area.value, 0.12566370614359172953850573)
         self.assertEqual(area.unit, 'm2')
-        self.assertEqual(area.uncert, np.sqrt((2 * np.pi / 4 * 0.4 * 0.002)**2))
-        
-        
-        
-        
-         
-        
+        self.assertEqual(area.uncert, np.sqrt((2 * np.pi / 4 * 0.4 * 0.002)**2))  
 
     def testCompare(self):
         a = variable(1, 'm')
         b = variable([2, 3, 4], 'm')
         np.testing.assert_equal(a < b, [True, True, True])
         np.testing.assert_equal(a <= b, [True, True, True])
         np.testing.assert_equal(a > b, [False, False, False])
         np.testing.assert_equal(a >= b, [False, False, False])
         np.testing.assert_equal(a == b, [False, False, False])
         np.testing.assert_equal(a != b, [True, True, True])
-
+        
         a = variable([2, 3, 4], 'm')
         b = variable(1, 'm')
         np.testing.assert_equal(a < b, [False, False, False])
         np.testing.assert_equal(a <= b, [False, False, False])
         np.testing.assert_equal(a > b, [True, True, True])
         np.testing.assert_equal(a >= b, [True, True, True])
         np.testing.assert_equal(a == b, [False, False, False])
         np.testing.assert_equal(a != b, [True, True, True])
 
         a = variable([1, 2], 'm')
         b = variable([2, 3, 4], 'm')
         with self.assertRaises(Exception) as context:
-            c = a < b
+            a < b
         self.assertTrue("operands could not be broadcast together with shapes (2,) (3,)" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a <= b
+            a <= b
         self.assertTrue("operands could not be broadcast together with shapes (2,) (3,)" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a > b
+            a > b
         self.assertTrue("operands could not be broadcast together with shapes (2,) (3,)" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a >= b
+            a >= b
         self.assertTrue("operands could not be broadcast together with shapes (2,) (3,)" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a == b
+            a == b
         self.assertTrue("operands could not be broadcast together with shapes (2,) (3,)" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a != b
+            a != b
         self.assertTrue("operands could not be broadcast together with shapes (2,) (3,)" in str(context.exception))
         
         
         a = variable(1, 'm')
         b = variable(2, 'C')
         with self.assertRaises(Exception) as context:
-            c = a < b
+            a < b
         self.assertTrue("You cannot compare 1 [m] and 2 [C] as they do not have the same SI base unit" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a <= b
+            a <= b
         self.assertTrue("You cannot compare 1 [m] and 2 [C] as they do not have the same SI base unit" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a > b
+            a > b
         self.assertTrue("You cannot compare 1 [m] and 2 [C] as they do not have the same SI base unit" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a >= b
+            a >= b
         self.assertTrue("You cannot compare 1 [m] and 2 [C] as they do not have the same SI base unit" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a == b
+            a == b
         self.assertTrue("You cannot compare 1 [m] and 2 [C] as they do not have the same SI base unit" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            c = a != b
+            a != b
         self.assertTrue("You cannot compare 1 [m] and 2 [C] as they do not have the same SI base unit" in str(context.exception))
 
         a = variable([1, 2, 3], 'm')
         b = variable([2, 3, 4], 'm')
         np.testing.assert_equal(a < b, [True, True, True])
         np.testing.assert_equal(a <= b, [True, True, True])
         np.testing.assert_equal(a > b, [False, False, False])
@@ -1472,26 +1472,25 @@
         a2 = variable(3, 'L/min', 0.3)
         b2 = variable(102, 'Pa', 4.7)
         a2.addCovariance(b2, 4, 'L-Pa/min')
         c2 = a2 * b2
         c2 *= a2
         
         np.testing.assert_equal(C[0].value, c0.value)
-        self.assertTrue(C._unitObject._assertEqual(c0.unit))
+        self.assertTrue(C._unitObject == unit(c0.unit))
         np.testing.assert_equal(C[0].uncert, c0.uncert)
         
         np.testing.assert_equal(C[1].value, c1.value)
-        self.assertTrue(C._unitObject._assertEqual(c0.unit))
+        self.assertTrue(C._unitObject == unit(c0.unit))
         np.testing.assert_equal(C[1].uncert, c1.uncert)
         
         np.testing.assert_equal(C[2].value, c2.value)
-        self.assertTrue(C._unitObject._assertEqual(c0.unit))
+        self.assertTrue(C._unitObject == unit(c0.unit))
         np.testing.assert_equal(C[2].uncert, c2.uncert)
-
-              
+      
     def testAppend(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(45, 'Pa', 1.2)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
 
         A_vec.append(A)
         np.testing.assert_equal(A_vec.value, [12.3, 54.3, 91.3, 12.3])
@@ -1517,31 +1516,30 @@
         d = variable([13, 14, 15], 'Pa')
         b.addCovariance(d, [0.1, 0.2, 0.3], 'm-Pa')
         a.append(b)
         c.append(d) 
         d = a * c
 
         np.testing.assert_equal(d.value, np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]))
-        self.assertTrue(d._unitObject._assertEqualStatic(d.unit, 'm-Pa'))        
-        np.testing.assert_equal(d.uncert, np.sqrt(2 * np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]) * np.array([0,0,0,0.1,0.2,0.3])))
+        self.assertTrue(d._unitObject == unit('m-Pa'))        
+        np.testing.assert_array_almost_equal(d.uncert, np.sqrt(2 * np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]) * np.array([0,0,0,0.1,0.2,0.3])))
         
         
         a = variable([1, 2, 3], 'm')
         b = variable([4, 5, 6], 'm')
         c = variable([10, 11, 12], 'Pa')
         d = variable([13, 14, 15], 'Pa')
         b.addCovariance(c, [0.1, 0.2, 0.3], 'm-Pa')
         a.append(b)
         c.append(d) 
         d = a * c
         np.testing.assert_equal(d.value, np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]))
-        self.assertTrue(d._unitObject._assertEqualStatic(d.unit, 'm-Pa'))        
+        self.assertTrue(d._unitObject == unit('m-Pa'))        
         np.testing.assert_equal(d.uncert, np.array([0,0,0,0,0,0]))
         
-        
     def testAddBel(self):
         a = variable(11,'dB', 0.1)
         b = variable(19,'dB',1.2)
         c = a + b
         self.assertEqual(c.value, 19.638920341433795986775635083534144311728776386508569289294)
         self.assertEqual(c.unit, 'dB')
         gradA = (10**(11/10)) / (10**(19/10) + 10**(11/10))
@@ -1757,17 +1755,16 @@
         b = variable(19,'ddec',1.2)
         c = b-a
         self.assertAlmostEqual(c.value, 18.250596325673850704123951198937009709734608031896818185442)
         self.assertEqual(c.unit, 'ddec')
         gradA = -10**(1.1+1) / (10**(19/10) - 10**1.1)
         gradB = 10**(19/10) / (10**(19/10) - 10**1.1)
         self.assertAlmostEqual(c.uncert, np.sqrt( (gradA * a.uncert)**2 + (gradB * b.uncert)**2))
-      
 
-    def testTemperatureArithmatic(self):
+    def testTemperatureAddition(self):
         a = variable(20,'C')
         b = variable(30,'C')
         c = a + b
         self.assertEqual(c.value, 50)
         self.assertEqual(c.unit, 'C')
         
         a = variable(20,'C')
@@ -1784,43 +1781,14 @@
         
         a = variable(20,'DELTAC')
         b = variable(30,'DELTAC')
         c = a + b
         self.assertEqual(c.value, 50)
         self.assertEqual(c.unit, 'DELTAC')
         
-        
-        a = variable(20,'C')
-        b = variable(30,'C')
-        c = a - b
-        self.assertEqual(c.value, -10)
-        self.assertEqual(c.unit, 'DELTAC')
-        
-        a = variable(20,'C')
-        b = variable(30,'DELTAC')
-        c = a - b
-        self.assertEqual(c.value, -10)
-        self.assertEqual(c.unit, 'C')
-        
-        a = variable(20,'DELTAC')
-        b = variable(30,'C')
-        with self.assertRaises(Exception) as context:
-            c = a - b
-        self.assertTrue("You tried to subtract a temperature from a temperature differnce. This is not possible." in str(context.exception))
-
-        
-        a = variable(20,'DELTAC')
-        b = variable(30,'DELTAC')
-        c = a - b
-        self.assertEqual(c.value, -10)
-        self.assertEqual(c.unit, 'DELTAC')
-        
-        
-        
-        
         a = variable(100,'K')
         b = variable(20, 'C')
         c = a + b 
         self.assertEqual(c.value, 100 + 273.15 + 20)
         self.assertEqual(c.unit, 'K')
         
         a = variable(100,'DELTAK')
@@ -1837,16 +1805,39 @@
         
         a = variable(100,'DELTAK')
         b = variable(20, 'DELTAC')
         c = a + b 
         self.assertEqual(c.value, 120)
         self.assertEqual(c.unit, 'DELTAK')
         
+    def testTemperatureSubtraction(self):
+        a = variable(20,'C')
+        b = variable(30,'C')
+        c = a - b
+        self.assertEqual(c.value, -10)
+        self.assertEqual(c.unit, 'DELTAC')
         
+        a = variable(20,'C')
+        b = variable(30,'DELTAC')
+        c = a - b
+        self.assertEqual(c.value, -10)
+        self.assertEqual(c.unit, 'C')
         
+        a = variable(20,'DELTAC')
+        b = variable(30,'C')
+        with self.assertRaises(Exception) as context:
+            c = a - b
+        self.assertTrue("You tried to subtract a temperature from a temperature differnce. This is not possible." in str(context.exception))
+
+        a = variable(20,'DELTAC')
+        b = variable(30,'DELTAC')
+        c = a - b
+        self.assertEqual(c.value, -10)
+        self.assertEqual(c.unit, 'DELTAC')
+              
         a = variable(100,'K')
         b = variable(20, 'C')
         c = a - b 
         self.assertEqual(c.value, 100 - ( 273.15 + 20))
         self.assertEqual(c.unit, 'DELTAK')
         
         a = variable(20, 'C')
@@ -1871,14 +1862,15 @@
         a = variable(100,'DELTAK')
         b = variable(20, 'DELTAC')
         c = a - b 
         self.assertEqual(c.value, 100 - 20)
         self.assertEqual(c.unit, 'DELTAK')
         
         
+    def testTemperatureMean(self):
         a = variable(20,'C')
         b = variable(30,'C')
         c = np.mean([a,b])
         self.assertEqual(c.value, 25)
         self.assertEqual(c.unit, 'C')
```

### Comparing `pyees-1.3.6/pyees/unit.py` & `pyees-1.3.7/pyees/unit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import numpy as np
-
+from fractions import Fraction
+from copy import copy
 
 class _unitConversion():
 
     def __init__(self, scale, offset=0) -> None:
         self.scale = scale
         self.offset = offset
 
-
-
     def __mul__(self, other):
         if isinstance(other, _unitConversion):
             scale = self.scale * other.scale
             offset = self.scale * other.offset + self.offset
         else:
             scale = self.scale * other
             offset = self.offset
@@ -25,15 +24,14 @@
         for _ in range(other):
             scale *= self.scale
             offset*= self.scale
             offset += self.offset
             
         return _unitConversion(scale, offset)
 
-
     def __truediv__(self, other):
         if isinstance(other, _unitConversion):
             return _unitConversion(1 / other.scale, - other.offset / other.scale) * self
         return self * _unitConversion(1 / other)
 
     def convert(self, value, useOffset=True):
         if useOffset:
@@ -224,26 +222,26 @@
     'kg-m2/s3-A2' : resistance,
     'm2/s' : kinematicViscosity,
     'Np': logrithmicUnits,
     'DELTAK': temperatureDifference
 }
 
 knownPrefixes = {
-    'T': 1e12,
-    'G': 1e9,
-    'M': 1e6,
-    'k': 1e3,
-    'h': 1e2,
-    'da': 1e1,
-    'd': 1e-1,
-    'c': 1e-2,
-    'm': 1e-3,
-    'mu': 1e-6,
-    'n': 1e-9,
-    'p': 1e-12
+    'T':10**12,
+    'G':10**9,
+    'M':10**6,
+    'k':10**3,
+    'h':10**2,
+    'da':10**1,
+    'd':10**-1,
+    'c':10**-2,
+    'm':10**-3,
+    'mu':10**-6,
+    'n':10**-9,
+    'p':10**-12
 }
 
 
 knownUnits = {}
 for key, d in knownUnitsDict.items():
     for item, _ in d.items():
         if item not in knownUnits:
@@ -301,39 +299,36 @@
             raise ValueError(f'The unit {p+newUnit} is already known within the unit system')
         unitPrefixCombinations.append(newUnit)
 
     ## create the conversion 
     conversion =  _unitConversion(scale, offset)
 
 
-    upper, upperPrefix,upperExp, lower, lowerPrefix, lowerExp = unit._getLists(existingUnit)
-    nUpper = len(upper)
-    units = upper + lower
-    exponents = upperExp + lowerExp
-    prefixes = upperPrefix + lowerPrefix
-    SIBaseUnitLists = [[],[]]
+    existingUnitDict = unit._getUnitDict(existingUnit)
+    existingUnitDictSI = unit._getUnitDictSI(existingUnitDict)
+    SIBaseUnit = unit._getUnitStrFromDict(existingUnitDictSI)
+        
     
-    for i, (u, exponent, prefix) in enumerate(zip(units, exponents, prefixes)):
-                
-        _SIBaseUnit, unitConversion = knownUnits[u]
-        unitConversion =  unitConversion ** exponent
+    for key, item in existingUnitDict.items():
+        for pre, exp in item.items():    
+                    
+            unitConversion = knownUnits[key][1]
+            
+            isUpper = exp > 0
+            
+            if not isUpper: exp *= -1
+            
+            unitConversion =  unitConversion ** exp
 
-        if exponent != 1: _SIBaseUnit += str(exponent)
-        
-        if not prefix is None: unitConversion *= knownPrefixes[prefix]
+            if not pre is None: unitConversion *= knownPrefixes[pre]
 
-        if i <= nUpper-1:
-            conversion = unitConversion * conversion
-            SIBaseUnitLists[0].append(_SIBaseUnit)
-        else:
-            conversion = _unitConversion(1) / unitConversion * conversion
-            SIBaseUnitLists[1].append(_SIBaseUnit)
-            
-    SIBaseUnit = '-'.join(SIBaseUnitLists[0])
-    if SIBaseUnitLists[1]: SIBaseUnit += '/' + '-'.join(SIBaseUnitLists[1])
+            if isUpper:
+                conversion = unitConversion * conversion
+            else:
+                conversion = _unitConversion(1) / unitConversion * conversion
     
     knownUnits[newUnit] = [SIBaseUnit, conversion]
         
     global knownCharacters
     for s in newUnit:
         knownCharacters.add(s)
 
@@ -341,201 +336,244 @@
 hyphen = '-'
 slash = '/'
 integers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
 
 
 class unit():
 
-    def __init__(self, unitStr) -> None:
-        if unitStr == '':
-            unitStr = '1'
+    def __init__(self, unitStr = None, unitDict = None):
+        if unitStr is None and unitDict is None:
+            unitStr = ''
         
-        # remove any unknown characters
-        unitStr = self._formatUnit(unitStr)
-
-        # split the unit in upper and lower
-        self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp = self._getLists(unitStr)
-
-        # create the unit string
-        self.unitStr = self._createUnitString()
-
-        self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
-        self._converterToSI = self._getConverter(*self._getLists(self._SIBaseUnit))
-
-    def _createUnitString(self):
-        return self._combineUpperAndLower(self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp)
-
-    @staticmethod
-    def _cancleUnits(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp):
-        # cancle the units
-        for indexUpper, up in enumerate(upper):
-            if up in lower:
-                indexLower = lower.index(up)
-
-                # only cancle units if they have the same prefix
-                if upperPrefix[indexUpper] == lowerPrefix[indexLower]:
-                    expUpper = upperExp[indexUpper]
-                    expLower = lowerExp[indexLower]
-
-                    # set the unit to '1'
-                    if expUpper == expLower:
-                        upper[indexUpper] = '1'
-                        lower[indexLower] = '1'
-                    elif expUpper < expLower:
-                        upper[indexUpper] = '1'
-                    else:
-                        lower[indexLower] = '1'
+        if not unitStr is None:
+            self.unitDict = self._getUnitDict(self._formatUnitStr(unitStr))
+        else:
+            self.unitDict = unitDict
+            
+        self.unitStr = self._getUnitStrFromDict(self.unitDict)
+        self.unitDictSI = self._getUnitDictSI(self.unitDict)
+        self.unitStrSI = self._getUnitStrFromDict(self.unitDictSI)
+        
+        # ## create a version of the self.unitDictSI that is formatted in the same way as a unitDict
+        # unitDictSI = {}
+        # for key, exp in self.unitDictSI.items():
+        #     u = knownUnits[key][0]
+        #     u,p,e = unit._splitUnitExponentAndPrefix(u)
+        #     unitDictSI[u] = {p: e*exp}
+        self._converterToSI = self.getConverterFromDict(self.unitDictSI)
 
-                    # reduce the exponent
-                    minExp = np.min([expUpper, expLower])
-                    lowerExp[indexLower] -= minExp
-                    upperExp[indexUpper] -= minExp
-
-        # remove '1' if the upper or lower is longer than 1
-        if len(upper) > 1:
-            indexesToRemove = [i for i, elem in enumerate(upper) if elem == '1']
-            upper = [elem for i, elem in enumerate(upper) if i not in indexesToRemove]
-            upperPrefix = [elem for i, elem in enumerate(upperPrefix) if i not in indexesToRemove]
-            upperExp = [elem for i, elem in enumerate(upperExp) if i not in indexesToRemove]
-        if len(lower) > 1:
-            indexesToRemove = [i for i, elem in enumerate(lower) if elem == '1']
-            lower = [elem for i, elem in enumerate(lower) if i not in indexesToRemove]
-            lowerPrefix = [elem for i, elem in enumerate(lowerPrefix) if i not in indexesToRemove]
-            lowerExp = [elem for i, elem in enumerate(lowerExp) if i not in indexesToRemove]
-
-        # return the list ['1'] if there are no more units
-        if not upper:
-            upper = ['1']
-            upperExp = ['1']
-        if not lower:
-            lower = ['1']
-            lowerExp = ['1']
-        return upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp
 
     @staticmethod
-    def _combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp):
-
-        upperPrefix = [elem if not elem is None else "" for elem in upperPrefix]
-        lowerPrefix = [elem if not elem is None else "" for elem in lowerPrefix]
-        upperExp = [str(elem) if elem != 1 else "" for elem in upperExp]
-        lowerExp = [str(elem) if elem != 1 else "" for elem in lowerExp]
-        upper = [pre + up + exp for pre, up, exp in zip(upperPrefix, upper, upperExp) if up != "1"]
-        lower = [pre + low + exp for pre, low, exp in zip(lowerPrefix, lower, lowerExp) if low != "1"]
+    def _getUnitStrFromDict(unitDict):
+        upper, lower = [], []
+        for u, item in unitDict.items():    
+            for p, exp in item.items():
+                if p is None: p = ''
 
-        # create a unit string
-        u = hyphen.join(upper) if upper else "1"
+                up = exp > 0
+                
+                if not up:
+                    exp *= -1
+                
+                if exp == 1:
+                    exp = ''
+                
+                s = f'{p}{u}{exp}'
+                if up:
+                    upper.append(s)
+                else:
+                    lower.append(s)
+                                
+        upper = '-'.join(upper)
+        
         if lower:
-            lower = hyphen.join(lower)
-            u = u + '/' + lower
-
-        return u
-
-    @staticmethod
-    def _multiply(a, b):
-
-        aUpper, aUpperPrefix, aUpperExp, aLower, aLowerPrefix, aLowerExp = unit._getLists(a)
-        bUpper, bUpperPrefix, bUpperExp, bLower, bLowerPrefix, bLowerExp = unit._getLists(b)
+            upper += '/' + '-'.join(lower)
+                
+        return upper
+      
+    def getUnitWithoutPrefix(self):
+        
+        upper, lower = [],[]
+        
+        for key, item in self.unitDict.items():
+            exp = sum(item.values())
+            isUpper = exp > 0
+            if not isUpper: exp *= -1
+            if exp == 1: exp = ''
+            s = f'{key}{exp}'
+            if isUpper:
+                upper.append(s)
+            else:
+                lower.append(s)
+        
+        out = '-'.join(upper)
+        if lower:
+            out += '/' + '-'.joing(lower)
+            
+        return out
+        
+    @ staticmethod
+    def _splitCompositeUnit(compositeUnit):
+        lower = []
+        if not slash in compositeUnit:
+            upper = compositeUnit.split(hyphen)
+            return upper, lower
+    
+        compositeUnit = compositeUnit.split(slash)
 
-        upper = aUpper + bUpper
-        upperPrefix = [elem if not elem is None else '' for elem in aUpperPrefix + bUpperPrefix]
-        upperExp = aUpperExp + bUpperExp
-        lower = aLower + bLower
-        lowerPrefix = [elem if not elem is None else '' for elem in aLowerPrefix + bLowerPrefix]
-        lowerExp = aLowerExp + bLowerExp
-
-        def reduceLists(units, unitPrefixes, unitExponents):
-            # combine the prefix and the unit
-            units = [pre + u for u, pre in zip(units, unitPrefixes)]
-
-            # loop over all unique combinations of prefix and units
-            setUnits = set(units)
-            tmpUnits = [''] * len(setUnits)
-            for i, u in enumerate(setUnits):
-                indexes = [_ for _, elem in enumerate(units) if elem == u]
-                exponent = sum([unitExponents[elem] for elem in indexes])
-                tmpUnits[i] = u
-
-                # add the exponent
-                if exponent != 1 and u != '1':
-                    tmpUnits[i] += str(exponent)
-
-            # split in to lists againt
-            tmpUnits = [unit._removeExponentFromUnit(elem) for elem in tmpUnits]
-            exponents = [elem[1] for elem in tmpUnits]
-            tmpUnits = [elem[0]for elem in tmpUnits]
-            tmpUnits = [unit._removePrefixFromUnit(elem) for elem in tmpUnits]
-            prefixes = [elem[1] for elem in tmpUnits]
-            units = [elem[0]for elem in tmpUnits]
-            return units, prefixes, exponents
-
-        upper, upperPrefix, upperExp = reduceLists(upper, upperPrefix, upperExp)
-        lower, lowerPrefix, lowerExp = reduceLists(lower, lowerPrefix, lowerExp)
-
-        upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp = unit._cancleUnits(
-            upper,
-            upperPrefix,
-            upperExp,
-            lower,
-            lowerPrefix,
-            lowerExp
-        )
+        if len(compositeUnit) > 2:
+            raise ValueError('A unit can only have a single slash (/)')
 
-        out = unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp)
+        upper = compositeUnit[0].split(hyphen)
+        lower = compositeUnit[1].split(hyphen) if len(compositeUnit) > 1 else []
 
-        return out
+        return upper, lower
 
     @staticmethod
     def _splitUnitExponentAndPrefix(unitStr):
         prefixUnit, exponent = unit._removeExponentFromUnit(unitStr)
         u, prefix = unit._removePrefixFromUnit(prefixUnit)
         return u, prefix, exponent
 
-
     @staticmethod
-    def _getLists(unitStr):
-        upper, lower = unit._splitCompositeUnit(unitStr)
+    def _reduceDict(unitDict):
+        
+        ## loop over all units, and remove any prefixes, which has an exponenet of 0
+        for key, item in unitDict.items():
+            prefixesToRemove = []
+            for pre, exp in item.items():
+                if exp == 0:
+                    prefixesToRemove.append(pre)
+            for pre in prefixesToRemove:
+                unitDict[key].pop(pre)
+    
+        ## remove the units, which has no items in their dictionary
+        keysToRemove = []
+        for key, item in unitDict.items():
+            if not item:
+                keysToRemove.append(key)
+        for key in keysToRemove:
+            unitDict.pop(key)
+        
+        ## remove the unit '1' above the fraction line, if there are any other units above the fraction line
+        keys = list(unitDict.keys())
+        if len(keys) > 1 and '1' in keys:
+            otherUpper = False
+            for key, item in unitDict.items():
+                if key == '1':
+                    continue
+                for pre, exp in item.items():
+                    if exp > 0:
+                        otherUpper = True
+                        break
+                if otherUpper:
+                    break
+            if otherUpper:
+                unitDict.pop('1')
                 
-        upper, upperPrefix, upperExp = map(list, zip(*[unit._splitUnitExponentAndPrefix(up) for up in upper]))
+        ## add the units '1' if there are not other units
+        if not unitDict:
+            unitDict = {'1': {None: 1}}
         
-        if lower:
-            lower, lowerPrefix, lowerExp = map(list, zip(*[unit._splitUnitExponentAndPrefix(low) for low in lower]))
-            upper = ['DELTA' + elem if elem in temperature else elem for elem in upper]
-            lower = ['DELTA' + elem if elem in temperature else elem for elem in lower]
-        else:
-            lowerPrefix = []
-            lowerExp = []
+        ## set the exponent of the unit '1' to 1
+        if '1' in unitDict:
+            unitDict['1'][None] = 1
+        
+        ## make temperature units in to temperature differences, if there are any other units in the dict
+        for temperatureUnit in temperature.keys():
+            if temperatureUnit in unitDict:
+                otherKeys = list(unitDict.keys())
+                otherKeys.remove(temperatureUnit)
+                if otherKeys:
+                    unitDict['DELTA' + temperatureUnit] = unitDict[temperatureUnit]
+                    unitDict.pop(temperatureUnit)
+        
+        
+        
+        return unitDict
+    
+    @staticmethod
+    def _getUnitDictSI(unitDict):
+        out = {}
+        for key, item in unitDict.items():
+            unitSI = knownUnits[key][0]
+            upper,lower = unit._splitCompositeUnit(unitSI)
+            nUpper = len(upper)
+            for exp in item.values():
+                for i, elem in enumerate(upper + lower):
+                    u,p,e = unit._splitUnitExponentAndPrefix(elem)
+                    if i > nUpper - 1:
+                        e *= -1
+                    if u in out:
+                        if p in out[u]:
+                            out[u][p] += e * exp
+                        else:
+                            out[u][p] = e * exp
+                    else:
+                        out[u] = {p: e * exp} 
+        out = unit._reduceDict(out)                 
+        return out
 
+    @staticmethod
+    def _getUnitDict(unitStr):
+        upper, lower = unit._splitCompositeUnit(unitStr)
 
-        return upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp
+        out = {}
+        
+        nUpper = len(upper)
+        for i, elem in enumerate(upper + lower):
+            
+            u, p, e = unit._splitUnitExponentAndPrefix(elem)
 
+            if i > nUpper - 1:
+                e *= -1
+            
+            if not u in out:
+                out[u] = {p: e}
+            else:
+                if not p in out[u]:
+                    out[u][p] = e
+                else:
+                    out[u][p] += e
+        
+        out = unit._reduceDict(out)
+        
+        return out
+   
     @ staticmethod
-    def _formatUnit(unitStr):
+    def _formatUnitStr(unitStr):
         
-        if unitStr is None:
-            return '1'
+        ## remove spaces
+        unitStr = unitStr.replace(' ', '')
         
-        # Removing any illegal symbols
+        # check for any illegal symbols
         for s in unitStr:
             if s not in knownCharacters:
                 raise ValueError(f'The character {s} is not used within the unitsystem')
+        
+        ## return the unity        
+        if unitStr is None or unitStr == '':
+            return '1'
 
         ## find start parenthesis is the unit string
         startParenIndexes = [i for i, s in enumerate(unitStr) if s == '(']
         stopParenIndexes = [i for i, s in enumerate(unitStr) if s == ')']
-
-        ## return if no parenthesis where found
+        
         if not startParenIndexes and not stopParenIndexes:
-            return unit.__formatUnit(unitStr)
+            unitStr = unitStr.split('-')
+            unitStr = [elem for elem in unitStr if not elem == '']
+            unitStr = '-'.join(unitStr) if unitStr else '1'
+            return unitStr
         
         ## check that the number of start and stop parenthesis are equal
         if len(startParenIndexes) != len(stopParenIndexes):
             raise ValueError('The unit string has to have an equal number of open parenthesis and close parenthesis')
         
         if len(startParenIndexes) == 1 and startParenIndexes[0] == 0 and stopParenIndexes[0] == len(unitStr) -1:
-            return unit._formatUnit(unitStr[startParenIndexes[0]+1:stopParenIndexes[0]])
+            return unit._formatUnitStr(unitStr[startParenIndexes[0]+1:stopParenIndexes[0]])
         
         ## find all parenthesis pairs
         allIndexes = startParenIndexes + stopParenIndexes
         allIndexes.sort()
         isStartParen = [elem in startParenIndexes for elem in allIndexes]
         done, iter, maxIter, parenOrder  = False, 0, len(allIndexes), []
         while not done:
@@ -550,150 +588,89 @@
 
             if len(allIndexes) == 0: break
             
             iter += 1
             if iter > maxIter:
                 raise ValueError('An order to evaluate the parenthesis could not be found')
         
+        
+        ## find any slashes outside of parenthesis
+        slashOutsideParensFound = False
+        index = -1
+        parenLevel = 0
+        for i, s in enumerate(unitStr):
+            if s == '(':
+                parenLevel += 1
+            elif s== ')':
+                parenLevel -= 1
+            
+            if parenLevel == 0 and s == '/':
+                if not slashOutsideParensFound:
+                    index = i
+                    slashOutsideParensFound = True
+                else:
+                    raise ValueError("You can only have a signle slash ('/') outside of parenthesis")
+        
+        if slashOutsideParensFound:
+            ## there was a slash outside of the parenthesis.
+            ## split the unitStr at the slash and return the upper divided by the lower
+            upper = unitStr[0:index]
+            lower = unitStr[index+1:]
+            upper = unit._getUnitDict(unit._formatUnitStr(upper))
+            lower = unit._getUnitDict(unit._formatUnitStr(lower))
+            return unit._getUnitStrFromDict(unit.staticTruediv(upper, lower))
+            
+        ## there were no slashes outside of the parenthesis
+        ## append the entire unit as a "parenthesis"
         parenOrder.append([0,len(unitStr)])
         
+        ## loop over the parenthesis from the inner parenthesis to the outer parenthesis
         for i in range(len(parenOrder)-1):
             currentParens = parenOrder[i]
-            nextParens = parenOrder[i+1]
             end = currentParens[1]
+            nextParens = parenOrder[i+1]
             
+            ## get the unitDict from the stringwithin the current parentheses
             _unitStr = unitStr[currentParens[0]+1:currentParens[1]]
             _unitStrLenOriginal = len(_unitStr)
-            _unitStr = unit._formatUnitStringWithParenthesis(_unitStr)
+            _unitStr = unit._formatUnitStr(_unitStr)
+            _unitDict = unit._getUnitDict(_unitStr)
+
+            ## determine if the nextparenthesis encompasses the current parenthesis
             if nextParens[0] <= currentParens[0] and nextParens[1]>=currentParens[1]:
+                
+                ## get the string from the end of the current parenthesis to the end of the next parenthesis
                 nextBit = unitStr[currentParens[1]+1:nextParens[1]]
-                exponent = nextBit.split('/')[0]
-                exponent = exponent.split('-')[0]
                 
+                ## A potential exponent of the current parenthis has to be
+                # above a potential slash (/) and before any potential hyphens (-)
+                exponent = nextBit.split('/')[0].split('-')[0]
+                
+                
+                ## try to cast the exponent to an integer
+                ## if this works, then raise the unitDict to the exponent
                 try:
                     exponent = int(exponent)
-                    upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp = unit._getLists(_unitStr)
-                    siBaseUnit = unit._getSIBaseUnit(upper, upperExp ,lower, lowerExp)
-                    _unitStr = unit.__staticPow(_unitStr, upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp, siBaseUnit, exponent)[0]
+                    _unitDict = unit.staticPow(_unitDict, None, _unitStr, exponent)
+                    _unitStr = unit._getUnitStrFromDict(_unitDict)
                     end += len(str(exponent))
                 except ValueError: pass
-            
-            _unitStrLenUpdate = len(_unitStr)
-            
-            dLen = _unitStrLenUpdate - _unitStrLenOriginal
-            for j in range(i, len(parenOrder)):
-                if parenOrder[j][0] >= currentParens[1]: parenOrder[j][0] += dLen
-                if parenOrder[j][1] >= currentParens[1]: parenOrder[j][1] += dLen-1
-            
-            unitStr = unitStr[0:currentParens[0]] + '(' + _unitStr + ')' + unitStr[end+1:]
-
-    
-        unitStr = unit._formatUnitStringWithParenthesis(unitStr)
-        
-        ## find start parenthesis is the unit string
-        startParenIndexes = [i for i, s in enumerate(unitStr) if s == '(']
-        stopParenIndexes = [i for i, s in enumerate(unitStr) if s == ')']
-        
-        ## check that the number of start and stop parenthesis are equal
-        if len(startParenIndexes) != len(stopParenIndexes):
-            raise ValueError('The unit string has to have an equal number of open parenthesis and close parenthesis')
-        
-        if len(startParenIndexes) == 0:
-            return unitStr
-        
-        done = False
-        while not done:
-            if unitStr[0] == '(' and unitStr[len(unitStr)-1] == ')':
-                unitStr = unitStr[1:len(unitStr)-1]
-            else:
-                break
-        
-        if '(' in unitStr or ')' in unitStr:    
-            raise ValueError('The unit could not be parsed')
         
-        return unitStr
 
-    
-    @staticmethod
-    def _formatUnitStringWithParenthesis(unitStr):
-        
-        ## determine if there is a slash outside of a parenthesis pair
-        tally = 0
-        for i, s in enumerate(unitStr):
-            if s == '/' and tally == 0:
+            ## update the next parenthesis based on the change of lengt of _unitStr
+            dLen = len(_unitStr) - _unitStrLenOriginal
+            for j in range(i+1, len(parenOrder)):
+                if parenOrder[j][0] >= currentParens[1]: parenOrder[j][0] += dLen-1
+                if parenOrder[j][1] >= currentParens[1]: parenOrder[j][1] += dLen-2
                 
-                a = unitStr[0:i]
-                b = unitStr[i+1:]
-                a = unit._formatUnit(a)
-                b = unit._formatUnit(b)
-                
-                aUpper, aUpperPrefix, aUpperExp, aLower, aLowerPrefix, aLowerExp = unit._getLists(a)
-                bUpper, bUpperPrefix, bUpperExp, bLower, bLowerPrefix, bLowerExp = unit._getLists(b)
-                
-                upper = aUpper + bLower
-                upperPrefix = aUpperPrefix + bLowerPrefix
-                upperExp = aUpperExp + bLowerExp
-                lower = aLower + bUpper
-                lowerPrefix = aLowerPrefix + bUpperPrefix
-                lowerExp = aLowerExp + bUpperExp
-                
-                return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix ,lowerExp)
-            
-            if s == '(':
-                tally += 1
-            if s == ')':
-                tally -= 1
-      
-        
-        return unit.__formatUnit(unitStr)
-            
-    @staticmethod
-    def __formatUnit(unitStr):
-        # Removing any spaces
-        unitStr = unitStr.replace(' ', '')
-        unitStr = unitStr.split('/')
-        
-        if len(unitStr)>2:
-            raise ValueError('A unit can only have a single slash (/)')
-        
-        if len(unitStr) > 1:
-            upper, lower = unitStr
-            lower = [elem for elem in lower.split('-') if elem != '']
-        else:
-            upper, lower = unitStr[0], []
-        
-        upper = [elem for elem in upper.split('-') if elem != '']
-        
-        if upper:
-            out = '-'.join(upper)
-        else:
-            out = '1'
-        
-        if lower:
-            out += '/' + '-'.join(lower)
-            
-        return out
-    
-    @ staticmethod
-    def _splitCompositeUnit(compositeUnit):
-        lower = []
-        if not slash in compositeUnit:
-            upper = compositeUnit.split(hyphen)
-            return upper, lower
-    
-        compositeUnit = compositeUnit.split(slash)
-
-        if len(compositeUnit) > 2:
-            raise ValueError('A unit can only have a single slash (/)')
-
-        upper = compositeUnit[0].split(hyphen)
-        lower = compositeUnit[1].split(hyphen) if len(compositeUnit) > 1 else []
-
-        return upper, lower
+            ## update unitStr
+            unitStr = unitStr[0:currentParens[0]] + _unitStr + unitStr[end+1:]
 
+        return unitStr
+ 
     @ staticmethod
     def _removeExponentFromUnit(u):
         
         integerIndexes = [i for i, char in enumerate(u) if char in integers]
         
         if not integerIndexes:
             return u, 1
@@ -714,36 +691,14 @@
             # No symbols are left after removing the integers
             if exponent != 1:
                 raise ValueError(f'The unit {u} was stripped of all integers which left no symbols in the unit. This is normally due to the integers removed being equal to 1, as the unit is THE unit. Howver, the intergers removed was not equal to 1. The unit is therefore not known.')
             u = '1'
         return u, exponent
 
     @staticmethod
-    def _assertEqualStatic(a, b):
-
-        aUpper, aLower = unit._splitCompositeUnit(a)
-        bUpper, bLower = unit._splitCompositeUnit(b)
-               
-        for elem in aUpper:
-            if not elem in bUpper:
-                return False
-            bUpper.remove(elem)
-        if bUpper:
-            return False
-        
-        for elem in aLower:
-            if not elem in bLower:
-                return False
-            bLower.remove(elem)
-        if bLower:
-            return False
-        
-        return True
-
-    @staticmethod
     def _removePrefixFromUnit(unit):
         
         if unit in knownUnits:
             return unit, None
 
         # The unit was not found. This must be because the unit has a prefix
         found = False
@@ -768,386 +723,289 @@
             raise ValueError(f'The unit ({prefix}) was not found. Therefore it was interpreted as a prefix and a unit. The prefix was identified as "{p}" and the unit was identified as "{unit}". However, the unit "1" cannot have a prefix')
 
         # look for the unit without the prefix
         if not unit in knownUnits:
             raise ValueError(f'The unit ({prefix}{unit}) was not found. Therefore it was interpreted as a prefix and a unit. However the unit ({unit}) was not found')
         return unit, prefix
 
-    @staticmethod
-    def _splitCompositeAndIncreaseExponent(unitStr, exp):
-            
-        up, low = unit._splitCompositeUnit(knownUnits[unitStr][0])
-        
-        up, upExp = map(list, zip(*[unit._removeExponentFromUnit(elem) for elem in up]))
-        low, lowExp = map(list, zip(*[unit._removeExponentFromUnit(elem) for elem in low])) if low else [[],[]]
-        
-        upExp = [elem * exp for elem in upExp]
-        lowExp = [elem * exp for elem in lowExp]
+    def __str__(self, pretty=False):
         
-        return up, upExp, low, lowExp
+        if not pretty:
+            return self.unitStr
 
-    @staticmethod
-    def _getSIBaseUnit(upper, upperExp, lower, lowerExp):    
-                
-        nUpper = len(upper)
-        upperOut, lowerOut, upperExpOut, lowerExpOut = [], [], [], []
-        
-        for i, (elem, exp) in enumerate(zip(upper + lower, upperExp + lowerExp)):
-            
-            up,low = unit._splitCompositeUnit(knownUnits[elem][0])
-            
-            if (i >= nUpper):
-                up, low = low, up
-            
-            for elem in up:
-                elem, elemExp = unit._removeExponentFromUnit(elem)
-                elemExp *= exp
-                if not elem in upperOut:
-                    upperOut.append(elem)
-                    upperExpOut.append(elemExp)
-                else:
-                    index = upperOut.index(elem)
-                    upperExpOut[index] += elemExp
-                    
-            for elem in low:
-                elem, elemExp = unit._removeExponentFromUnit(elem)
-                elemExp *= exp
-                if not elem in lowerOut:
-                    lowerOut.append(elem)
-                    lowerExpOut.append(elemExp)
+        upper, lower = [],[]
+        for u, item in self.unitDict.items():
+            for pre, exp in item.items():
+                isUpper = exp > 0
+                if not isUpper: exp *= -1 
+                if exp == 1: exp = ''
+                if pre == None: pre = ''
+                s = f'{pre}{u}{exp}'
+                if isUpper:
+                    upper.append(s)
                 else:
-                    index = lowerOut.index(elem)
-                    lowerExpOut[index] += elemExp
+                    lower.append(s)
         
+        if not lower:
+            # no fraction
+            out = '\cdot'.join(upper)
+            return out
         
-        upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp = unit._cancleUnits(
-            upperOut, [None] * len(upperOut), upperExpOut, lowerOut, [None] * len(lowerOut), lowerExpOut
-        )
-
-        return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp)
-
-    def isCombinationUnit(self):
-        if len(self.upper) > 1:
-            return True
-        if self.lower:
-            return True
-        return False
+        # a fraction is needed
+        out = rf'\frac{{'
+        out += '\cdot'.join(upper)
+        out += rf'}}{{'
+        out += '\cdot'.join(lower)
+        out += rf'}}'
+        return out
 
-    def __str__(self, pretty=False):
-        if not pretty:
-            return self.unitStr
-        else:
-            if self.lower:
-                # a fraction is needed
-                out = rf'\frac{{'
-                for i, (up, prefix, exp) in enumerate(zip(self.upper, self.upperPrefix, self.upperExp)):
-                    if exp > 1:
-                        up = rf'{up}^{exp}'
-                    if prefix is None:
-                        prefix = ''
-                    out += rf'{prefix}{up}'
-                    if i != len(self.upper) - 1:
-                        out += rf' \cdot '
-                out += rf'}}{{'
-                for i, (low, prefix, exp) in enumerate(zip(self.lower, self.lowerPrefix, self.lowerExp)):
-                    if exp > 1:
-                        low = rf'{low}^{exp}'
-                    if prefix is None:
-                        prefix = ''
-                    out += rf'{prefix}{low}'
-                    if i != len(self.lower) - 1:
-                        out += rf' \cdot '
-                out += rf'}}'
-            else:
-                # no fraction
-                out = r''
-                for i, (up, prefix, exp) in enumerate(zip(self.upper, self.upperPrefix, self.upperExp)):
-                    if exp > 1:
-                        up = rf'{up}^{exp}'
-                    if prefix is None:
-                        prefix = ''
-                    out += rf'{prefix}{up}'
-                    if i != len(self.upper) - 1:
-                        out += rf' \cdot '
-            return out
+    def __eq__(self, other):
+        return self.unitDict == other.unitDict
 
-    def _assertEqual(self, other):
-        if isinstance(other, unit):
-            other = other.unitStr
-        return self._assertEqualStatic(self.unitStr, other)
+    def isLogarithmicUnit(self):
+        upper, lower = unit._splitCompositeUnit(self.unitStr)
+        if lower or len(upper) != 1: return False
+        return unit._splitUnitExponentAndPrefix(upper[0])[0] in logrithmicUnits
 
     def __add__(self, other):
-        
-        ## output 1: are the units a logarithmic unit
-        ## output 2: outputUnit
-        ## output 3: scaleToSI. If true, then scale both self and other to SI and neglect output 2 and 3
-        ## output 4: scaleSelf. If true then scale self to remove the prefix
-        ## output 5: scaleOther. If true then scale other to remove the prefix
-        
         ## determine the units of self without any prefixes and convert this to a string
-        selfWithoutPrefixes = unit(unit._combineUpperAndLower(self.upper, [None] * len(self.upperPrefix), self.upperExp, self.lower, [None] * len(self.lowerPrefix), self.lowerExp))
-        selfWithoutPrefixesString = str(selfWithoutPrefixes)
-        
-        ## determine if self is a part of the logarithmic units
-        isLogarithmicUnit = selfWithoutPrefixesString in logrithmicUnits.keys()
+        selfUnitDictWithoutPrefixes = {}
+        for key, item in self.unitDict.items():
+            selfUnitDictWithoutPrefixes[key] = {}
+            selfUnitDictWithoutPrefixes[key][None] = 0
+            for exp in item.values():
+                selfUnitDictWithoutPrefixes[key][None] += exp
         
         ## determine if self is the same as other - then no conversions are necessary
-        if unit._assertEqualStatic(str(self), str(other)):
-            return isLogarithmicUnit, str(self), False, False, False   
+        if self.unitDict == other.unitDict:
+            return unit(unitDict=self.unitDict)  
         
         ## determine the units of other without any prefixes and convert this to a string
-        otherWithoutPrefixes = unit(unit._combineUpperAndLower(other.upper, [None] * len(other.upperPrefix), other.upperExp, other.lower, [None] * len(other.lowerPrefix), other.lowerExp))
-        otherWithoutPrefixesString = str(otherWithoutPrefixes)
-        
-        ## determine if self and/or other has to be scaled in order to remove any prefixes
-        scaleSelf = str(self) != selfWithoutPrefixesString
-        scaleOther = str(other) != otherWithoutPrefixesString
+        otherUnitDictWithoutPrefixes = {}
+        for key, item in other.unitDict.items():
+            otherUnitDictWithoutPrefixes[key] = {}
+            otherUnitDictWithoutPrefixes[key][None] = 0
+            for exp in item.values():
+                otherUnitDictWithoutPrefixes[key][None] += exp
         
         ## determine if the self and other are identical once any prefixes has been removed
-        if unit._assertEqualStatic(selfWithoutPrefixesString, otherWithoutPrefixesString):
-            return isLogarithmicUnit, selfWithoutPrefixesString, False, scaleSelf, scaleOther
+        if selfUnitDictWithoutPrefixes == otherUnitDictWithoutPrefixes:
+            return unit(unitDict=selfUnitDictWithoutPrefixes)
         
         # determine if the SI base units of self and other are equal
-        if self._SIBaseUnit == other._SIBaseUnit:
-            return isLogarithmicUnit, self._SIBaseUnit, True, False, False
+        if self.unitDictSI == other.unitDictSI:
+            return unit(unitDict=copy(self.unitDictSI))
         
         ## determine if "DELTAK" and "K" are the SI Baseunits of self and other
-        SIBaseUnits = [selfWithoutPrefixes._SIBaseUnit,  otherWithoutPrefixes._SIBaseUnit]        
-        if 'DELTAK' in SIBaseUnits and 'K' in SIBaseUnits:
+        SIBaseUnits = [self.unitDictSI, other.unitDictSI]        
+        if {'DELTAK':{None:1}} in SIBaseUnits and {'K':{None:1}} in SIBaseUnits:
             
-            indexTemp = SIBaseUnits.index('K')
+            indexTemp = SIBaseUnits.index({'K':{None:1}})
             indexDiff = 0 if indexTemp == 1 else 1
             
-            units = [selfWithoutPrefixesString, otherWithoutPrefixesString]
+            units = [list(selfUnitDictWithoutPrefixes.keys())[0], list(otherUnitDictWithoutPrefixes.keys())[0]]
 
             if units[indexTemp] == units[indexDiff][-1]:        
-                return isLogarithmicUnit, units[indexTemp], False, scaleSelf, scaleOther
+                return unit(unitDict=[selfUnitDictWithoutPrefixes, otherUnitDictWithoutPrefixes][indexTemp])
             
-            return isLogarithmicUnit, 'K', True, False, False
+            return unit('K')
 
         raise ValueError(f'You tried to add a variable in [{self}] to a variable in [{other}], but the units do not have the same SI base unit')
 
     def __sub__(self, other):
-        ## output 1: are the units a logarithmic unit
-        ## output 2: outputUnit
-        ## output 3: scaleToSI. If true, then scale both self and other to SI and neglect output 2 and 3
-        ## output 4: scaleSelf. If true then scale self to remove the prefix
-        ## output 5: scaleOther. If true then scale other to remove the prefix
-        
-        ## determine the units of self without any prefixes and convert this to a string
-        selfWithoutPrefixes = unit(unit._combineUpperAndLower(self.upper, [None] * len(self.upperPrefix), self.upperExp, self.lower, [None] * len(self.lowerPrefix), self.lowerExp))
-        selfWithoutPrefixesString = str(selfWithoutPrefixes)
         
-        ## determine if self is a part of the logarithmic units
-        isLogarithmicUnit = selfWithoutPrefixesString in logrithmicUnits.keys()
+        ## determine the units of self without any prefixes
+        selfUnitDictWithoutPrefixes = {}
+        for key, item in self.unitDict.items():
+            selfUnitDictWithoutPrefixes[key] = {}
+            selfUnitDictWithoutPrefixes[key][None] = 0
+            for exp in item.values():
+                selfUnitDictWithoutPrefixes[key][None] += exp
+        
+        
+        ## determine the units of other without any prefixes and convert
+        otherUnitDictWithoutPrefixes = {}
+        for key, item in other.unitDict.items():
+            otherUnitDictWithoutPrefixes[key] = {}
+            otherUnitDictWithoutPrefixes[key][None] = 0
+            for exp in item.values():
+                otherUnitDictWithoutPrefixes[key][None] += exp
         
-        ## determine the units of other without any prefixes and convert this to a string
-        otherWithoutPrefixes = unit(unit._combineUpperAndLower(other.upper, [None] * len(other.upperPrefix), other.upperExp, other.lower, [None] * len(other.lowerPrefix), other.lowerExp))
-        otherWithoutPrefixesString = str(otherWithoutPrefixes)
         
-        ## determine if self and/or other has to be scaled in order to remove any prefixes
-        scaleSelf = str(self) != selfWithoutPrefixesString
-        scaleOther = str(other) != otherWithoutPrefixesString
-
         ## determine if "DELTAK" and "K" are the SI Baseunits of self and other
-        SIBaseUnits = [self._SIBaseUnit, other._SIBaseUnit]
-        if SIBaseUnits[0] == 'K' and SIBaseUnits[1] == 'K':
-            if selfWithoutPrefixesString == otherWithoutPrefixesString:
-                return isLogarithmicUnit, 'DELTA' + str(self), False, scaleSelf, scaleOther
-            return isLogarithmicUnit,'DELTAK', True, False, False
+        SIBaseUnits = [self.unitDictSI, other.unitDictSI]        
+        if SIBaseUnits[0] == {'K':{None:1}} and SIBaseUnits[1] == {'K':{None:1}}:
+            if self.unitDict == other.unitDict:
+                return unit(unitDict = copy(self.unitDict))
+            return unit('K')
 
-        if 'DELTAK' in SIBaseUnits and 'K' in SIBaseUnits:
-            
-            indexTemp = SIBaseUnits.index('K')
+        if {'DELTAK':{None:1}} in SIBaseUnits and {'K':{None:1}} in SIBaseUnits:
+            indexTemp = SIBaseUnits.index({'K':{None:1}})
             if indexTemp != 0:
-                raise ValueError('You tried to subtract a temperature from a temperature differnce. This is not possible.')
-            indexDiff = 0 if indexTemp == 1 else 1
-            
-            units = [selfWithoutPrefixesString, otherWithoutPrefixesString]
-
-
-            if units[indexTemp] == units[indexDiff][-1]:        
-                return isLogarithmicUnit, units[indexTemp], False, scaleSelf, scaleOther
-            
-            return isLogarithmicUnit, 'K', True, False, False
+                raise ValueError('You tried to subtract a temperature from a temperature differnce. This is not possible.')      
+            return unit(unitDict=[selfUnitDictWithoutPrefixes, otherUnitDictWithoutPrefixes][indexTemp])
         
                 
         ## determine if self is the same as other - then no conversions are necessary
-        if unit._assertEqualStatic(str(self), str(other)):
-            return isLogarithmicUnit, str(self), False, False, False
-           
-        ## determine if the self and other are identical once any prefixes has been removed
-        if unit._assertEqualStatic(selfWithoutPrefixesString, otherWithoutPrefixesString):
-            return isLogarithmicUnit, selfWithoutPrefixesString, False, scaleSelf, scaleOther
+        if self.unitDict == other.unitDict:
+            return unit(unitDict=self.unitDict)
         
-        # test if the SI base units are identical
-        if self._SIBaseUnit == other._SIBaseUnit:
-            return isLogarithmicUnit, self._SIBaseUnit, True, False, False
+        ## determine if the self and other are identical once any prefixes has been removed
+        if selfUnitDictWithoutPrefixes == otherUnitDictWithoutPrefixes:
+            return unit(unitDict=selfUnitDictWithoutPrefixes)
         
+        # determine if the SI base units of self and other are equal
+        if self.unitDictSI == other.unitDictSI:
+            return unit(unitDict=self.unitDictSI)
         
         
         raise ValueError(f'You tried to subtract a variable in [{other}] from a variable in [{self}], but the units do not have the same SI base unit')
 
     def __mul__(self, other):
-        return unit._multiply(self.unitStr, other.unitStr)
-
+        out = {}
+        
+        for key, item in self.unitDict.items():
+            out[key]= {}
+            for pre, exp in item.items():
+                out[key][pre] = exp
+        
+        for key, item in other.unitDict.items():
+            if not key in out:
+                out[key] = item
+            else:
+                for pre, exp in item.items():
+                    if not pre in out[key]:
+                        out[key][pre] = exp
+                    else:
+                        out[key][pre] += exp
+        
+        out = unit._reduceDict(out)
+        return unit(unitDict = out)
+    
     def __truediv__(self, other):
+        return unit(unitDict = unit.staticTruediv(self.unitDict, other.unitDict))
+    
+    @staticmethod
+    def staticTruediv(a, b):
+        out = {}
         
-        a = self.unitStr
-        b = other.unitStr
-
-        bUpper, bUpperPrefix, bUpperExp, bLower, bLowerPrefix, bLowerExp = unit._getLists(b)
-
-        b = self._combineUpperAndLower(
-            upper=bLower,
-            upperPrefix=bLowerPrefix,
-            upperExp=bLowerExp,
-            lower=bUpper,
-            lowerPrefix=bUpperPrefix,
-            lowerExp=bUpperExp
-        )
-
-        return unit._multiply(a, b)
-
+        for key, item in a.items():
+            out[key]= {}
+            for pre, exp in item.items():
+                out[key][pre] = exp
+        
+        for key, item in b.items():
+            if not key in out:
+                out[key] = {}
+                for pre, exp in item.items():
+                    out[key][pre] = -1 * exp
+            else:
+                for pre, exp in item.items():
+                    if not pre in out[key]:
+                        out[key][pre] = -exp
+                    else:
+                        out[key][pre] -= exp
+        
+        return unit._reduceDict(out)
+    
     def __pow__(self, power):
-        return self.__staticPow(self.unitStr, self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp, self._SIBaseUnit, power)
+        return unit(unitDict= unit.staticPow(self.unitDict, self.unitDictSI, self.unitStr, power))
     
     @staticmethod
-    def __staticPow(unitStr, upper, upperPrefix, upperExp ,lower, lowerPrefix, lowerExp, _SIBaseUnit, power):
-        if power == 0:
-            return '1', False
-
-        elif power > 1:
-
-            if unitStr == '1':
-                # self is '1'. Therefore the power does not matter
-                return unitStr, False
-
-            else:
-                # self is not '1'. Therefore all exponents are multiplied by the power
-
-                if not (isinstance(power, int) or power.is_integer()):
-                    raise ValueError('The power has to be an integer')
-
-                upperExp = [int(elem * power) for elem in upperExp]
-                lowerExp = [int(elem * power) for elem in lowerExp]
-
-                return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp) , False
-
-        else:
-            # the power is smaller than 1.
-            # Therefore it is necessary to determine if all exponents are divisible by the recibricol of the power
-
-            if unitStr == '1':
-                # self is '1'. Therefore the power does not matter
-                return unitStr, False
-            else:
-                # self is not '1'.
-                # Therefore it is necessary to determine if all exponents are divisible by the recibricol of the power
-
-                def isCloseToInteger(a, rel_tol=1e-9, abs_tol=0.0):
-                    b = np.around(a)
-                    return abs(a - b) <= max(rel_tol * max(abs(a), abs(b)), abs_tol)
-                
-                # Test if the exponent of all units is divisible by the power
-                try:
-                    for exp in upperExp + lowerExp:
-                        if not isCloseToInteger(exp * power):
-                            raise ValueError(f'You can not raise a variable with the unit {unitStr} to the power of {power}')
-
-                    upperExp = [int(elem * power) for elem in upperExp]
-                    lowerExp = [int(elem * power) for elem in lowerExp]
-
-                    return unit._combineUpperAndLower(upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp), False
-                
-                except ValueError:                
-                    ## the exponents of the unit was not divisible by the power
-                    ## test if the exponents of the SIBaseunit is divisible by the power 
-                    
-                    siUpper, siUpperPrefix, siUpperExp, siLower, siLowerPrefix, siLowerExp = unit._getLists(_SIBaseUnit)
-                    for exp in siUpperExp + siLowerExp:
-                        if not isCloseToInteger(exp * power):
-                            raise ValueError(f'You can not raise a variable with the unit {unitStr} to the power of {power}')
-
-                    siUpperExp = [int(elem * power) for elem in siUpperExp]
-                    siLowerExp = [int(elem * power) for elem in siLowerExp]
-
-                    return unit._combineUpperAndLower(siUpper, siUpperPrefix, siUpperExp, siLower, siLowerPrefix, siLowerExp), True
-
-    def getConverter(self, newUnit):
-        newUnit = unit._formatUnit(newUnit)
-
-        # get the upper, upperExp, lower and lowerExp of the newUnit without creating a unit
-        otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(newUnit)
-
-        # determine if the SI bases are identical
-        otherSIBase = self._getSIBaseUnit(otherUpper, otherUpperExp, otherLower, otherLowerExp)
+    def staticPow(unitDict, unitDictSI, unitStr, power):
         
-        if unit._assertEqualStatic(self._SIBaseUnit, otherSIBase) == False:
-            raise ValueError(f'You tried to convert from {self} to {newUnit}. But these do not have the same base units')
+        if unitDict == {'1': {None: 1}}:
+            return unitDict
         
-        return self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
-
-    def getUnitWithoutPrefix(self):
-        return self._removePrefixFromUnit(self.unitStr)[0]
+        frac = Fraction(power).limit_denominator()
+        num, den = frac._numerator, frac._denominator
+        
+        ## determine if it is possible to take the power of the unitDict
+        isPossible = True
+        out = {}
+        for key, item in unitDict.items():
+            for pre, exp in item.items():
+                if not (exp * num) % den == 0:
+                    isPossible = False
+                    break
+            if not isPossible:
+                break
+        
+        ## if it is possible, then return a new unitDict
+        if isPossible:
+            for key, item in unitDict.items():
+                out[key] = {}
+                for pre, exp in unitDict[key].items():
+                    out[key][pre] = int(num * exp / den)
+            out = unit._reduceDict(out)
+            return out
+        
+        ## determine if it is possible to take the power of the sibase unit
+        isPossible = True
+        out = {}
+        for key, item in unitDictSI.items():
+            for pre, exp in item.items():
+                if not (exp * num) % den == 0:
+                    isPossible = False
+                    break
+            
+        ## if it is possible, then return a new unitDict
+        if isPossible:
+            for key, item in unitDictSI.items():
+                out[key] = {}
+                for pre, exp in item.items():
+                    out[key][pre] = int(num * exp / den)
+            out = unit._reduceDict(out)
+            return out
+        
+        raise ValueError(f'You can not raise a variable with the unit {unitStr} to the power of {power}')
 
-    def getLogarithmicConverter(self, unitStr = None):
-        if unitStr is None:
-            unitStr = self.unitStr
-        u, p = self._removePrefixFromUnit(unitStr)
-        return knownUnits[u][1]
-   
-    def _getConverter(self, otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp):
+    def getConverter(self, newUnitStr):  
+        newUnitStr =  unit._formatUnitStr(newUnitStr)
+        newUnitDict = unit._getUnitDict(newUnitStr)
+        newUnitDictSI = unit._getUnitDictSI(newUnitDict)
+        if not (self.unitDictSI == newUnitDictSI):
+            raise ValueError(f'You tried to convert from {self} to {newUnitStr}. But these do not have the same base units')
+        return self.getConverterFromDict(newUnitDict)
+    
+    def getConverterFromDict(self, newUnitDict):    
         
         # initialize the scale and offset
         out = _unitConversion(1, 0)
-
-        nUpper = len(self.upper)
-        units = self.upper + self.lower 
-        prefixes = self.upperPrefix + self.lowerPrefix
-        exponents = self.upperExp + self.lowerExp
-        for i, (unit, prefix, exp) in enumerate(zip(units, prefixes, exponents)):
-            conv = knownUnits[unit][1]
-            if not prefix is None:
-                conv *= knownPrefixes[prefix]
-            if exp > 1: conv = conv ** exp
-            out = out * conv if i < nUpper else out / conv
-
-        nUpper = len(otherUpper)
-        units = otherUpper + otherLower
-        prefixes = otherUpperPrefix + otherLowerPrefix
-        exponents = otherUpperExp + otherLowerExp
-        for i, (unit, prefix, exp) in enumerate(zip(units, prefixes, exponents)):
-            conv = knownUnits[unit][1]
-            if not prefix is None:
-                conv *= knownPrefixes[prefix]
-            if exp > 1: conv = conv ** exp
-            out = out / conv if i < nUpper else out * conv
-
+        
+        ## loop over self.unitDict
+        for u, item in self.unitDict.items():
+            for pre, exp in item.items():
+                conv = knownUnits[u][1]
+                if not pre is None: conv *= knownPrefixes[pre]
+                isUpper = exp > 0
+                if not isUpper: exp *= -1                    
+                conv = conv ** exp
+                out = out * conv if isUpper else out / conv
+
+        ## loop over newUnitDict
+        for u, item in newUnitDict.items():
+            for pre, exp in item.items():
+                conv = knownUnits[u][1]
+                if not pre is None: conv *= knownPrefixes[pre]
+                isUpper = exp > 0
+                if not isUpper: exp *= -1
+                conv = conv ** exp
+                out = out * conv if not isUpper else out / conv
+        
         return out
 
-    def convert(self, unitStr):
-        if unitStr == '':
-            unitStr = '1'
-
-        # remove any unknown characters
-        unitStr = self._formatUnit(unitStr)
-
-        # split the unit in upper and lower
-        self.upper, self.upperPrefix, self.upperExp, self.lower, self.lowerPrefix, self.lowerExp = self._getLists(unitStr)
-
-        # create the unit string
-        self.unitStr = self._createUnitString()
-
-        self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
-        otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
-        self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
-
-
+    def isCombinationUnit(self):
+        return len(list(self.unitDict.keys())) > 1
 
+    def getLogarithmicConverter(self, unitStr = None):
+        if unitStr is None:
+            unitStr = self.unitStr
+        u, _ = self._removePrefixFromUnit(unitStr)
+        return knownUnits[u][1]
 
-if __name__ == "__main__":
-    a = unit('%')
-    b = unit('%')
     
-    c = a + b
-    print(c)
+if __name__ == "__main__":
+    a = unit('K')
+    converter = a.getConverter('C')
+    print(converter.convert(300), 26.85)
+
```

### Comparing `pyees-1.3.6/pyees/variable.py` & `pyees-1.3.7/pyees/variable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from copy import copy
 import numpy as np
 try:
     from unit import unit
-    from unit import logrithmicUnits
 except ImportError:
     from pyees.unit import unit
-    from pyees.unit import logrithmicUnits
-    
-        
+     
     
 class logarithmicVariables:
     def __init__(self):
         pass
     
     @staticmethod
     def __add__(a,b):
@@ -125,15 +122,15 @@
     def uncert(self):
         return self._uncert
 
     def convert(self, newUnit):
         converter = self._unitObject.getConverter(newUnit)
         self._value = converter.convert(self._value, useOffset=not self._unitObject.isCombinationUnit())
         self._uncert = converter.convert(self._uncert, useOffset=False)
-        self._unitObject.convert(newUnit)
+        self._unitObject = unit(newUnit)
  
     def printUncertanty(self, value, uncert):
         # function to print number
         if uncert == 0 or uncert is None or np.isnan(uncert):
             return f'{value:.{self.nDigits}g}', None
 
         digitsUncert = -int(np.floor(np.log10(np.abs(uncert))))
@@ -195,14 +192,15 @@
         value, uncert = self.printUncertanty(value, uncert)
         if uncert is None:
             return rf'{value}{space}{unitStr}'
         else:
                 return rf'{value} {pm} {uncert}{space}{unitStr}'
 
     def _addDependent(self, var, grad):
+                
         # scale the gradient to SI units. This is necessary if one of the variables are converted after the dependency has been noted
         grad *= self._converterToSI.convert(1, useOffset=False) / var._converterToSI.convert(1, useOffset=False)
         
         if var.dependsOn:
             # the variable depends on other variables
             # loop over the dependencies of the variables and add them to the dependencies of self.
             # this ensures that the product rule is used
@@ -234,239 +232,239 @@
     def addCovariance(self, var, covariance: float, unitStr: str):
         try:
             float(covariance)
         except TypeError:
             raise ValueError(f'You tried to set the covariance between {self} and {var} with a non scalar value')
         
         covUnit = unit(unitStr)
-        selfVarUnit = unit(self._unitObject * var._unitObject)
-        if not unit._assertEqualStatic(covUnit._SIBaseUnit, selfVarUnit._SIBaseUnit):
+        selfVarUnit = self._unitObject * var._unitObject
+        if not covUnit.unitDictSI ==  selfVarUnit.unitDictSI:
             raise ValueError(f'The covariance of {covariance} [{unitStr}] does not match the units of {self} and {var}')
         
-        covariance *= covUnit._converterToSI.convert(1, useOffset=False)
+        covariance = covUnit._converterToSI.convert(covariance, useOffset=False)
         
         self.covariance[var] = covariance        
         var.covariance[self] = covariance
         
     def _calculateUncertanty(self):
- 
+        
+        ## all variances are determined in the SI unit system.
+        ## these has to be converted back in the the unit of self
+        scale = 1 / self._converterToSI.convert(1, useOffset=False) ** 2
+        
         # variance from each measurement
-        variance = 0
-
-        # loop over each different variable object in the dependency dict
-        for dependency in self.dependsOn.values():
-            
-            ## loop over each "instance" of the variable
-            ## an instance occurs when the variable has been changed using methods as __setitem__
-            ## this affectively makes the variable a "new" variable in the eyes of other variables
-    
-            ## add the variance constribution to the variance
-            unc, grad = dependency[0], dependency[1]
-            variance += (unc * grad) ** 2
-        
-        ## scale the variance back in to the currenct unit
-        ## the scaling is raised to a power of 2, as the above line should be
-        ## variance += (scale * unc * grad) ** 2
-        scale = 1 / self._converterToSI.convert(1, useOffset=False)
-        variance *= scale ** 2
+        variance = sum([(unc * grad)**2 for unc, grad in self.dependsOn.values()]) * scale
         
         # variance from the corralation between measurements
         ## covariance = list(vari, vari.currentValue, vari.currentUncert, varj, varj.currentValue, varj.currenctUncert, cov)
         ## from the above the gradients can be found from self.dependsOn
-        
         for var1 in self.dependsOn.keys():
             for var2 in var1.covariance.keys():
                 if var2 in self.dependsOn:
                     grad1 = self.dependsOn[var1][1]
                     grad2 = self.dependsOn[var2][1]
-                    s = scale**2 
                     cov = var1.covariance[var2]
-                    term = s * grad1 * grad2 * cov
-                    variance += term
-                    # variance += scale**2 * grad1 * grad2 * var1.covariance[var2]
+                    variance += scale * grad1 * grad2 * cov
 
         self._uncert = np.sqrt(variance)
         
     def __add__(self, other):
         
         if not isinstance(other, scalarVariable):
             return self + variable(other, self.unit)
 
         # determine if the two variable can be added
-        isLogarithmicUnit, outputUnit, scaleToSI, scaleSelf, scaleOther = self._unitObject + other._unitObject
-        if isLogarithmicUnit:
+        outputUnit = self._unitObject + other._unitObject
+        
+        ## handle logarithmic addition seperately
+        if outputUnit.isLogarithmicUnit():
             return logarithmicVariables.__add__(self, other)
 
-        # convert self and other to the SI unit system
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
-        
-        if scaleToSI:
-            self.convert(self._unitObject._SIBaseUnit)
-            other.convert(other._unitObject._SIBaseUnit)
-        else:
-            if scaleSelf:
-                a, _ = self._unitObject._removePrefixFromUnit(self.unit)
-                self.convert(a)
-            if scaleOther:
-                a, _ = other._unitObject._removePrefixFromUnit(other.unit)
-                other.convert(a)
-        
+        # convert self and other
+        selfUnit = copy(self._unitObject)
+        otherUnit = copy(other._unitObject)
+        
+        ## convert the units if the SI unit is identical to that of the output unit and the unit is not equal to the output unit
+        if self._unitObject.unitDictSI == outputUnit.unitDictSI and not self._unitObject == outputUnit:
+            self.convert(str(outputUnit))
+        if other._unitObject.unitDictSI == outputUnit.unitDictSI and not other._unitObject == outputUnit:
+            other.convert(str(outputUnit))
 
-        # determine the value and gradients
+        # determine the value
         val = self.value + other.value
         
-        # create the new variable
+        # create the new variable and add the self and other as dependencies
         var = variable(val, outputUnit)
         var._addDependent(self, 1)
         var._addDependent(other, 1)
         var._calculateUncertanty()
 
         # convert all units back to their original units
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        
-        ## convert the variable in to the original unit if self and other has the same original unit
-        ## otherwise keep the variable in the SI unit system
-        if (selfUnit == otherUnit):
-            var.convert(selfUnit)
-        
-        if outputUnit == 'K':
-            SIBaseUnits = [self._unitObject._SIBaseUnit, other._unitObject._SIBaseUnit]
-            if 'DELTAK' in SIBaseUnits and 'K' in SIBaseUnits:
-                var.convert([selfUnit, otherUnit][SIBaseUnits.index('K')]) 
+        if not self._unitObject == selfUnit:
+            self.convert(str(selfUnit))
+        if not other._unitObject == otherUnit:
+            other.convert(str(otherUnit))
+        
+        ## if the output unit is 'K' and one of the inputs is a temperature and the other is a tempreature difference
+        ## then return the output in the same unit as the temperature
+        ## this has no affect if the inputs are in 'K' and 'DeltaK'
+        ## but the output is converted to 'C' if the inputs are in 'C' and 'DeltaK' 
+        SIBaseUnits = [self._unitObject.unitDictSI, other._unitObject.unitDictSI]
+        if outputUnit.unitDict == {'K':{None:1}} and {'DELTAK':{None:1}} in SIBaseUnits and {'K':{None:1}} in SIBaseUnits:
+            var.convert(str([selfUnit, otherUnit][SIBaseUnits.index({'K':{None:1}})])) 
+            
         return var
 
     def __radd__(self, other):
         return self + other
 
     def __sub__(self, other):
         if not isinstance(other, scalarVariable):
             return self - variable(other, self.unit)
 
         # determine if the variables can be subtracted
-        isLogarithmicUnit, outputUnit, scaleToSI, scaleSelf, scaleOther = self._unitObject - other._unitObject
-        if isLogarithmicUnit:
+        outputUnit = self._unitObject - other._unitObject
+    
+        ## handle logarithmic unit seperately
+        if outputUnit.isLogarithmicUnit():
             return logarithmicVariables.__sub__(self, other)
-
-        # convert self and other to the SI unit system
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
- 
-        if scaleToSI:
-            self.convert(self._unitObject._SIBaseUnit)
-            other.convert(other._unitObject._SIBaseUnit)
-        else:
-            if scaleSelf:
-                a, _ = self._unitObject._removePrefixFromUnit(self.unit)
-                self.convert(a)
-            if scaleOther:
-                a, _ = other._unitObject._removePrefixFromUnit(other.unit)
-                other.convert(a)
-
-        # determine the value and gradients
+        
+        # convert self and other
+        selfUnit = copy(self._unitObject)
+        otherUnit = copy(other._unitObject)
+        
+        ## convert the units if the SI unit is identical to that of the output unit and the unit is not equal to the output unit
+        if self._unitObject.unitDictSI == outputUnit.unitDictSI and not self._unitObject == outputUnit:
+            self.convert(str(outputUnit))
+        if other._unitObject.unitDictSI == outputUnit.unitDictSI and not other._unitObject == outputUnit:
+            other.convert(str(outputUnit))
+       
+        # determine the value
         val = self.value - other.value
 
-        # create the new variable
+        # create the new variable and add the self and other as dependencies
         var = variable(val, outputUnit)
         var._addDependent(self, 1)
         var._addDependent(other, -1)
         var._calculateUncertanty()
 
-
-        # convert self and other back
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-
-        if self.unit == other.unit and outputUnit == self.unit:
-            var.convert(self.unit)
-        if outputUnit == 'K':
-            SIBaseUnits = [self._unitObject._SIBaseUnit, other._unitObject._SIBaseUnit]
-            if 'DELTAK' in SIBaseUnits and 'K' in SIBaseUnits:
-                var.convert([selfUnit, otherUnit][SIBaseUnits.index('K')]) 
+        # convert all units back to their original units
+        if not self._unitObject == selfUnit:
+            self.convert(str(selfUnit))
+        if not other._unitObject == otherUnit:
+            other.convert(str(otherUnit))
+
+        SIBaseUnits = [self._unitObject.unitDictSI, other._unitObject.unitDictSI]
+        if outputUnit.unitDictSI == {'K':{None:1}} and SIBaseUnits[0] == {'K':{None:1}} and SIBaseUnits[1] == {'K':{None:1}}:
+            if list(self._unitObject.unitDict.keys())[0] == list(other._unitObject.unitDict.keys())[0]:
+                var._unitObject = unit('DELTA' + list(self._unitObject.unitDict.keys())[0])
+            else:
+                var._unitObject = unit('DELTAK')
+            
         return var
 
     def __rsub__(self, other):
         return - self + other
 
     def __mul__(self, other):
     
         if not isinstance(other, scalarVariable):
             return self * variable(other)
 
+        ## determine the value
         val = self.value * other.value
+        
+        ## determine the output unit
         outputUnit = self._unitObject * other._unitObject
 
+        ## create a variable
         var = variable(val, outputUnit)
         var._addDependent(self, other.value)
         var._addDependent(other, self.value)
         var._calculateUncertanty()
 
-        if var._unitObject._SIBaseUnit == '1' and var._unitObject != '1':
+        ## if all units were cancled during the multiplication, then convert to 1
+        ## this will remove any remaining prefixes
+        if var._unitObject.unitDictSI == {'1':{None:1}} and var._unitObject.unitDict != {'1' : {None: 1}}:
             var.convert('1')
 
         return var
 
     def __rmul__(self, other):
         return self * other
 
     def __pow__(self, other):
+        
         if not isinstance(other, scalarVariable):
             return self ** variable(other, '')
 
         if str(other.unit) != '1':
             raise ValueError('The exponent can not have a unit')
 
-        selfUnit = copy(self.unit)
-        outputUnit, hasToBeScaledToSI = self._unitObject ** other.value
-
+        ## determine the output unit
+        outputUnit = self._unitObject ** other.value
+        
+        ## if self._unitObject has the same keys, as the output unit
+        ## then self does not have to be scaled to the SI unit system in order for the unit to be raised to the power
+        hasToBeScaledToSI = self._unitObject.unitDict.keys() != outputUnit.unitDict.keys()
         if hasToBeScaledToSI:
-            self.convert(self._unitObject._SIBaseUnit)
+            selfUnit = copy(self.unit)
+            self.convert(self._unitObject.unitStrSI)
         
+        ## dertermine the value
         val = self.value ** other.value
 
+        ## determine the gradients of the output with respoect to self and other
         def gradSelf(valSelf, valOTher):
             if valSelf != 0:
                 return  valOTher * valSelf ** (valOTher - 1)
             return 0
         
         def gradOther(valSelf, valOther, uncertOther):
             if uncertOther != 0:
                 return valSelf ** valOther * np.log(valSelf)
             return 0
         
         gradOther = np.vectorize(gradOther, otypes=[float])(self.value, other.value, other._uncert)
         gradSelf = np.vectorize(gradSelf, otypes=[float])(self.value, other.value)
         
+        ## create a new variable
         var = variable(val, outputUnit)
         var._addDependent(self, gradSelf)
         var._addDependent(other, gradOther)
         var._calculateUncertanty()
-        
+
+        ## converte self back if it was converted to the SI unit system
         if hasToBeScaledToSI:
             self.convert(selfUnit)
-        
+
         return var
 
     def __rpow__(self, other):
         return variable(other, '1') ** self
 
     def __truediv__(self, other):
         if not isinstance(other, scalarVariable):
             return self / variable(other)
-
+        
+        ## determine the value
         val = self.value / other.value
+        
+        ## determine the output unit
         outputUnit = self._unitObject / other._unitObject
 
+        ## create a variable
         var = variable(val, outputUnit)
         var._addDependent(self, 1 / other.value)
         var._addDependent(other, -self.value / (other.value**2))
         var._calculateUncertanty()
 
-        if var._unitObject._SIBaseUnit == '1' and var._unitObject != '1':
+        ## if all units were cancled during the multiplication, then convert to 1
+        ## this will remove any remaining prefixes
+        if var._unitObject.unitDictSI == {'1':{None:1}} and var._unitObject.unitDict != {'1' : {None: 1}}:
             var.convert('1')
 
         return var
 
     def __rtruediv__(self, other):
         if not isinstance(other, scalarVariable):
             return variable(other) / self
@@ -515,33 +513,33 @@
     def exp(self):
         return np.e**self
 
     def sqrt(self):
         return self**(1 / 2)
 
     def sin(self):
-        if str(self._unitObject._SIBaseUnit) != 'rad':
+        if self._unitObject.unitDictSI != {'rad': {None:1}}:
             raise ValueError('You can only take sin of an angle')
         
         outputUnit = '1'
-        if self._unitObject._assertEqual('rad'):
+        if self.unit == 'rad':
             val = np.sin(self.value)
             grad = np.cos(self.value)
         else:
             val = np.sin(np.pi / 180 * self.value)
             grad = np.pi / 180 * np.cos(np.pi / 180 * self.value)
         
         var = variable(val, outputUnit)
         var._addDependent(self, grad)
         var._calculateUncertanty()
 
         return var
 
     def cos(self):
-        if str(self._unitObject._SIBaseUnit) != 'rad':
+        if self._unitObject.unitDictSI != {'rad': {None:1}}:
             raise ValueError('You can only take cos of an angle')
 
         outputUnit = '1'
         if self.unit == 'rad':
             val = np.cos(self.value)
             grad = -np.sin(self.value)
         else:
@@ -551,15 +549,15 @@
         var = variable(val, outputUnit)
         var._addDependent(self, grad)
         var._calculateUncertanty()
 
         return var
 
     def tan(self):
-        if str(self._unitObject._SIBaseUnit) != 'rad':
+        if self._unitObject.unitDictSI != {'rad': {None:1}}:
             raise ValueError('You can only take tan of an angle')
 
         outputUnit = '1'
         if self.unit == 'rad':
             val = np.tan(self.value)
             grad = 2 / (np.cos(2 * self.value) + 1)
         else:
@@ -590,137 +588,78 @@
     
     def min(self):
         return self
     
     def mean(self):
         return self
 
-    def __lt__(self, other):
-        if not isinstance(other, scalarVariable):
-            return self < variable(other, self.unit)
-
-        if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
-            raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
+    @staticmethod
+    def __comparer__(func):
         
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
+        def wrap(*args):
+            a = args[0]
+            b = args[1]           
+            
+            if not isinstance(b,scalarVariable):
+                b = variable(b, a.unit)
+            
+            if a.unit == b.unit:
+                return func(a,b)
+            
+            if not a._unitObject.unitDictSI == b._unitObject.unitDictSI:
+                raise ValueError(f'You cannot compare {a} and {b} as they do not have the same SI base unit')
         
-        self.convert(self._unitObject._SIBaseUnit)
-        other.convert(self._unitObject._SIBaseUnit)
+            aUnit = copy(a.unit)
+            bUnit = copy(b.unit)
+            
+            a.convert(a._unitObject.unitStrSI)
+            b.convert(b._unitObject.unitStrSI)
+            
+            res = func(a,b)
+            
+            a.convert(aUnit)
+            b.convert(bUnit)
+            
+            return res
+            
+        return wrap
 
-        out = self.value < other.value
+    @__comparer__
+    def __lt__(self, other):
+        return self.value < other.value
         
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        return out
-
+    @__comparer__
     def __le__(self, other):
-        if not isinstance(other, scalarVariable):
-            return self <= variable(other, self.unit)
-        if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
-            raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
-        
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
-        
-        self.convert(self._unitObject._SIBaseUnit)
-        other.convert(self._unitObject._SIBaseUnit)
+        return self.value <= other.value
         
-        out = self.value <= other.value
-        
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        return out
-    
+    @__comparer__
     def __gt__(self, other):
-        if not isinstance(other, scalarVariable):
-            return self > variable(other, self.unit)
-
-        if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
-            raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
-        
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
-        
-        self.convert(self._unitObject._SIBaseUnit)
-        other.convert(self._unitObject._SIBaseUnit)
-
-        out = self.value > other.value
+        return self.value > other.value
            
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        return out
-   
+    @__comparer__
     def __ge__(self, other):
-        if not isinstance(other, scalarVariable):
-            return self >= variable(other, self.unit)
-
-        if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
-            raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
-        
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
-        
-        self.convert(self._unitObject._SIBaseUnit)
-        other.convert(self._unitObject._SIBaseUnit)
-
-        out = self.value >= other.value
-        
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        return out
-
+        return self.value >= other.value
+    
+    @__comparer__
     def __eq__(self, other):
-        if not isinstance(other, scalarVariable):
-            return self == variable(other, self.unit)
-
-        if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
-            raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
-        
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
-        
-        self.convert(self._unitObject._SIBaseUnit)
-        other.convert(self._unitObject._SIBaseUnit)
-        
         if isinstance(self, arrayVariable) and isinstance(other, arrayVariable):
             if len(self) != len(other):
-                raise ValueError(f"operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}")    
-        out = self.value == other.value
+                raise ValueError(f"operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}")   
+        return self.value == other.value
             
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        return out
-
+    @__comparer__
     def __ne__(self, other):
-        if not isinstance(other, scalarVariable):
-            return self != variable(other, self.unit)
-
-        if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
-            raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
-        
-        selfUnit = copy(self.unit)
-        otherUnit = copy(other.unit)
-        
-        self.convert(self._unitObject._SIBaseUnit)
-        other.convert(self._unitObject._SIBaseUnit)
-
         if isinstance(self, arrayVariable) and isinstance(other, arrayVariable):
             if len(self) != len(other):
-                raise ValueError(f"operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}")    
-        out = self.value != other.value
+                raise ValueError(f"operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}")   
+        return  self.value != other.value
             
-        self.convert(selfUnit)
-        other.convert(otherUnit)
-        return out
-
     def __hash__(self):
         return id(self)
 
-
 class arrayVariable(scalarVariable):
     
     def __init__(self, value = None, unitStr = None, uncert= None, nDigits= None, scalarVariables = None) -> None:
         
         if not (value is None) and not (scalarVariables is None):
             raise ValueError('You cannot supply both values and scalarVariables')
         
@@ -895,14 +834,17 @@
         if isinstance(other, arrayVariable):
             if len(self) != len(other):
                 raise ValueError(f'operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}')
             out = [a**b for a,b in zip(self, other)]
         else:
             out = [a**other for a in self]
 
+        ## if other is an arrayVariable, then this could imply that the unit of each element in out are not equal
+        ## if the units of the scalarVariables are equel, then collect them in an arrayVariable
+        ## else return the list of scalarVariables
         if all([out[0].unit == elem.unit for elem in out]):
             return arrayVariable(scalarVariables=out)
         
         return out
      
     def __rpow__(self,other):
         if not (isinstance(other, scalarVariable) or isinstance(other, arrayVariable)):
@@ -949,15 +891,15 @@
         return sum(self) / len(self)
     
     def convert(self, newUnit):
         converter = self._unitObject.getConverter(newUnit)
         for elem in self.scalarVariables:
             elem._value = converter.convert(elem._value, useOffset=not self._unitObject.isCombinationUnit())
             elem._uncert = converter.convert(elem._uncert, useOffset=False)
-        self._unitObject.convert(newUnit)
+        self._unitObject = unit(newUnit)
 
     def __iter__(self):
         self.n = 0
         return self
 
     def __next__(self):
         if self.n < len(self):
@@ -1002,13 +944,20 @@
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')      
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
-
-
 if __name__ == "__main__":
-    A = variable(7, '%', 0.1)
-    B = -A
-    print(B)
+    a = variable(23, 'deg', 2)
+    # a = variable(np.pi / 180 * 23, 'rad', np.pi /  180 *2)
+    b = np.sin(a)
+    print(b.dependsOn[a])
+    a.convert('rad')
+    print(b.dependsOn[a])
+    c = a * b
+    
+    
+    val = np.pi / 180 * 23
+    unc = np.pi / 180 * 2
+    print(c.uncert, np.sqrt((unc * (np.sin(val) + val * np.cos(val)))**2))
```

### Comparing `pyees-1.3.6/pyees.egg-info/PKG-INFO` & `pyees-1.3.7/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.6
+Version: 1.3.7
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.6/setup.py` & `pyees-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.6',
+    version='1.3.7',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

