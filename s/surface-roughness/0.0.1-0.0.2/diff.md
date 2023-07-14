# Comparing `tmp/surface-roughness-0.0.1.tar.gz` & `tmp/surface-roughness-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surface-roughness-0.0.1.tar", last modified: Fri Jul 14 17:59:27 2023, max compression
+gzip compressed data, was "surface-roughness-0.0.2.tar", last modified: Fri Jul 14 18:39:50 2023, max compression
```

## Comparing `surface-roughness-0.0.1.tar` & `surface-roughness-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:27.654648 surface-roughness-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 17:59:27.654648 surface-roughness-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:59:27.654648 surface-roughness-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:27.646648 surface-roughness-0.0.1/surface_roughness/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:27.654648 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/Directional.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/Directional.h
--rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/DirectionalRoughness.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/DirectionalRoughness.h
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/DirectionalUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/MeanApparentDip.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/MeanApparentDip.h
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness.h
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.h
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.h
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_cppimpl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:27.654648 surface-roughness-0.0.1/surface_roughness/_roughness_pyimpl/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_pyimpl/_DirectionalRoughness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_pyimpl/_TINBasedRoughness.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_roughness_pyimpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/_sampling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/roughness.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/roughness_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34662 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/surface_roughness/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:27.650648 surface-roughness-0.0.1/surface_roughness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 17:59:27.000000 surface-roughness-0.0.1/surface_roughness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 17:59:27.000000 surface-roughness-0.0.1/surface_roughness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:59:27.000000 surface-roughness-0.0.1/surface_roughness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:59:27.000000 surface-roughness-0.0.1/surface_roughness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 17:59:27.000000 surface-roughness-0.0.1/surface_roughness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:59:27.000000 surface-roughness-0.0.1/surface_roughness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:27.654648 surface-roughness-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-14 17:59:11.000000 surface-roughness-0.0.1/tests/test_geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:39:50.549680 surface-roughness-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 18:39:50.549680 surface-roughness-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:39:50.549680 surface-roughness-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:39:50.545680 surface-roughness-0.0.2/surface_roughness/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:39:50.545680 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/Directional.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/Directional.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/DirectionalRoughness.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/DirectionalRoughness.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/DirectionalUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/MeanApparentDip.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/MeanApparentDip.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_cppimpl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:39:50.545680 surface-roughness-0.0.2/surface_roughness/_roughness_pyimpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_pyimpl/_DirectionalRoughness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_pyimpl/_TINBasedRoughness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_roughness_pyimpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/_sampling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/roughness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/roughness_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34662 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/surface_roughness/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:39:50.545680 surface-roughness-0.0.2/surface_roughness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 18:39:50.000000 surface-roughness-0.0.2/surface_roughness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-14 18:39:50.000000 surface-roughness-0.0.2/surface_roughness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:39:50.000000 surface-roughness-0.0.2/surface_roughness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:39:50.000000 surface-roughness-0.0.2/surface_roughness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 18:39:50.000000 surface-roughness-0.0.2/surface_roughness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 18:39:50.000000 surface-roughness-0.0.2/surface_roughness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:39:50.549680 surface-roughness-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-14 18:39:34.000000 surface-roughness-0.0.2/tests/test_geometry_utils.py
```

### Comparing `surface-roughness-0.0.1/setup.py` & `surface-roughness-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     language='c++',
     extra_compile_args=cpp_args,
     extra_link_args=linkargs
 )
 
 setup(
     name="surface-roughness",
-    version="0.0.1",
+    version="0.0.2",
     description="Surface roughness calculation with Python",
     long_description=(Path(__file__).parent/"README.md").read_text(),
     author="Earl Magsipoc",
     author_email="e.magsipoc@mail.utoronto.ca",
     url="https://github.com/e-mags/pysurfaceroughness",
     license="MIT",
     package_dir = {
@@ -74,8 +74,8 @@
         'matplotlib',
         'mplstereonet',
         'shapely'
     ],
     cmdclass={"build_ext":build_ext},
     zip_safe=False,
     python_requires=">=3.7"
-)
+)
```

### Comparing `surface-roughness-0.0.1/surface_roughness/_geometry_utils.py` & `surface-roughness-0.0.2/surface_roughness/_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_profile.py` & `surface-roughness-0.0.2/surface_roughness/_profile.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/Directional.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/Directional.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/Directional.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/Directional.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/DirectionalRoughness.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/DirectionalRoughness.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/DirectionalRoughness.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/DirectionalRoughness.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/DirectionalUtil.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/DirectionalUtil.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/MeanApparentDip.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/MeanApparentDip.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/MeanApparentDip.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/MeanApparentDip.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_againstshear.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.h` & `surface-roughness-0.0.2/surface_roughness/_roughness_cpp/TINBasedRoughness_bestfit.h`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_cppimpl.cpp` & `surface-roughness-0.0.2/surface_roughness/_roughness_cppimpl.cpp`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_pyimpl/_DirectionalRoughness.py` & `surface-roughness-0.0.2/surface_roughness/_roughness_pyimpl/_DirectionalRoughness.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_roughness_pyimpl/_TINBasedRoughness.py` & `surface-roughness-0.0.2/surface_roughness/_roughness_pyimpl/_TINBasedRoughness.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/_sampling_utils.py` & `surface-roughness-0.0.2/surface_roughness/_sampling_utils.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/roughness.py` & `surface-roughness-0.0.2/surface_roughness/roughness.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/roughness_impl.py` & `surface-roughness-0.0.2/surface_roughness/roughness_impl.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness/sampling.py` & `surface-roughness-0.0.2/surface_roughness/sampling.py`

 * *Files identical despite different names*

### Comparing `surface-roughness-0.0.1/surface_roughness.egg-info/SOURCES.txt` & `surface-roughness-0.0.2/surface_roughness.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 surface_roughness/__init__.py
 surface_roughness/_geometry_utils.py
 surface_roughness/_profile.py
```

### Comparing `surface-roughness-0.0.1/tests/test_geometry_utils.py` & `surface-roughness-0.0.2/tests/test_geometry_utils.py`

 * *Files identical despite different names*

