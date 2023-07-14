# Comparing `tmp/multipoles-0.3.4.tar.gz` & `tmp/multipoles-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipoles-0.3.4.tar", last modified: Thu Jul  6 12:00:59 2023, max compression
+gzip compressed data, was "multipoles-0.4.0.tar", last modified: Fri Jul 14 10:05:33 2023, max compression
```

## Comparing `multipoles-0.3.4.tar` & `multipoles-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-06 12:00:59.848210 multipoles-0.3.4/
--rw-r--r--   0 mbaer    (671849960) 579947404     1070 2023-07-06 09:50:10.000000 multipoles-0.3.4/LICENSE
--rw-r--r--   0 mbaer    (671849960) 579947404      815 2023-07-06 12:00:59.848446 multipoles-0.3.4/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     4677 2023-07-06 09:50:10.000000 multipoles-0.3.4/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-06 12:00:59.844660 multipoles-0.3.4/multipoles/
--rw-r--r--   0 mbaer    (671849960) 579947404       66 2023-07-06 11:59:20.000000 multipoles-0.3.4/multipoles/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404    14360 2023-07-06 11:58:57.000000 multipoles-0.3.4/multipoles/expansion.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-06 12:00:59.847508 multipoles-0.3.4/multipoles.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404      815 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      252 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       12 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       11 2023-07-06 12:00:59.000000 multipoles-0.3.4/multipoles.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       79 2023-07-06 12:00:59.849334 multipoles-0.3.4/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404      968 2023-07-06 11:59:15.000000 multipoles-0.3.4/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-14 10:05:33.312928 multipoles-0.4.0/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1070 2023-07-06 09:50:10.000000 multipoles-0.4.0/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404      815 2023-07-14 10:05:33.313087 multipoles-0.4.0/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     4677 2023-07-06 09:50:10.000000 multipoles-0.4.0/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-14 10:05:33.309999 multipoles-0.4.0/multipoles/
+-rw-r--r--   0 mbaer    (671849960) 579947404       66 2023-07-14 10:04:33.000000 multipoles-0.4.0/multipoles/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404    16087 2023-07-14 10:04:22.000000 multipoles-0.4.0/multipoles/expansion.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-14 10:05:33.312539 multipoles-0.4.0/multipoles.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404      815 2023-07-14 10:05:33.000000 multipoles-0.4.0/multipoles.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      252 2023-07-14 10:05:33.000000 multipoles-0.4.0/multipoles.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-14 10:05:33.000000 multipoles-0.4.0/multipoles.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       12 2023-07-14 10:05:33.000000 multipoles-0.4.0/multipoles.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       11 2023-07-14 10:05:33.000000 multipoles-0.4.0/multipoles.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       79 2023-07-14 10:05:33.314535 multipoles-0.4.0/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404      968 2023-07-14 10:04:39.000000 multipoles-0.4.0/setup.py
```

### Comparing `multipoles-0.3.4/LICENSE` & `multipoles-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multipoles-0.3.4/PKG-INFO` & `multipoles-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipoles
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package for multipole expansions of electrostatic or gravitational potentials
 Home-page: https://github.com/maroba/multipoles
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: multipole expansion,physics,scientific-computing
 Platform: UNKNOWN
```

### Comparing `multipoles-0.3.4/README.md` & `multipoles-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `multipoles-0.3.4/multipoles/expansion.py` & `multipoles-0.4.0/multipoles/expansion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import numbers
 from scipy.special import sph_harm
 from scipy.integrate import simpson
 
 
 class MultipoleExpansion(object):
     """
     Perform a multipole expansion for a given charge or mass distribution.
@@ -258,32 +259,64 @@
     def eval(self, xyz, l_max=None):
         """
         Evaluate multipole expansion at a point with given coordinates.
 
         Parameters
         ----------
 
-        xyz: 3-tuple of floats
+        xyz: 3-tuple of (floats or arrays)
             The x,y,z coordinates of the points where to evaluate the expansion.
+            If three floats are given, then only one point with coordinates (x, y, z)
+            is evaluated. If three arrays xyz=(x, y, z) are given, the evaluation is done at each
+            point (x[i], y[i], z[i]).
 
         l_max: int, optional
             The maximum angular momentum to use for the expansion. If no value
             is given, use l_max from the original computation of the expansion.
             If l_max is given, only use contributions up to this angular momentum
             in the evaluation.
         """
         if l_max is None:
             l_max = self.l_max
         if l_max > self.l_max:
             raise ValueError(
                 "Multipole expansion only contains multipoles up to l_max={}.".format(self.l_max)
             )
-        contribs = self._multipole_contribs(xyz)
-        return sum(contribs[:l_max + 1])
-
+        assert isinstance(xyz, tuple) and len(xyz) == 3
+        
+        if any(hasattr(item, "__len__") for item in xyz): # some args are array-like            
+            # All passed arrays must have same length. Validate this and determine this
+            # length.
+            len_array = None            
+            for item in xyz:
+                if hasattr(item, "__len__"):
+                    if len_array is None:
+                        len_array = len(item)
+                    else:
+                        if len(item) != len_array:
+                            raise ValueError(f"All arrays must have the same length. Received: {len_array} != {len(item)}")                    
+            
+            # If numbers are passed along with arrays, expand the numbers to constant
+            # arrays of the right size.
+            xyz = list(xyz)
+            for i in range(3):                
+                if isinstance(xyz[i], numbers.Number):
+                    xyz[i] = np.ones(len_array) * xyz[i]
+            xyz = tuple(xyz)
+            
+            # Now do the evaluation
+            return np.array(
+                [sum(self._multipole_contribs((x, y, z))[:l_max + 1]) for x, y, z in zip(*xyz)]
+            )
+        elif all(isinstance(item, numbers.Number) for item in xyz):
+            # only numbers were passed; evaluate at single point      
+            return sum(self._multipole_contribs(xyz)[:l_max + 1])        
+        else:            
+            raise ValueError("Only triple of floats or tripe of arrays allowed.")
+        
     def _multipole_contribs(self, xyz):
         if not isinstance(xyz, np.ndarray):
             xyz = np.array(xyz)
 
         xyz_internal = xyz - self.center_of_charge
         r, phi, theta = cartesian_to_spherical(*xyz_internal)
```

### Comparing `multipoles-0.3.4/multipoles.egg-info/PKG-INFO` & `multipoles-0.4.0/multipoles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipoles
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package for multipole expansions of electrostatic or gravitational potentials
 Home-page: https://github.com/maroba/multipoles
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: multipole expansion,physics,scientific-computing
 Platform: UNKNOWN
```

### Comparing `multipoles-0.3.4/setup.py` & `multipoles-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='multipoles',
-    version='0.3.4',
+    version='0.4.0',
     description='A Python package for multipole expansions of electrostatic or gravitational potentials',
     long_description="""*multipoles* is a Python package for multipole expansions of the solutions of the Poisson equation     
        (e.g. electrostatic or gravitational potentials). It can handle discrete and continuous charge or mass distributions.
     """,
 
     license='MIT',
     url='https://github.com/maroba/multipoles',
```

