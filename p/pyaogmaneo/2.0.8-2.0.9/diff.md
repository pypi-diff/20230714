# Comparing `tmp/pyaogmaneo-2.0.8.tar.gz` & `tmp/pyaogmaneo-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.8.tar", last modified: Mon Jun 26 20:10:26 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.0.9.tar", last modified: Sat Jul  1 20:12:05 2023, max compression
```

## Comparing `pyaogmaneo-2.0.8.tar` & `pyaogmaneo-2.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.8/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-26 20:00:45.000000 pyaogmaneo-2.0.8/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.8/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.8/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.8/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-26 20:10:25.000000 pyaogmaneo-2.0.8/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.8/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-26 20:01:06.000000 pyaogmaneo-2.0.8/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-26 20:10:25.999165 pyaogmaneo-2.0.8/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8213 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8969 2023-06-26 18:24:52.000000 pyaogmaneo-2.0.8/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.9/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-01 20:10:42.000000 pyaogmaneo-2.0.9/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.9/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.9/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.9/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.9/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-01 20:06:13.000000 pyaogmaneo-2.0.9/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8213 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     9041 2023-06-30 23:06:07.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.8/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.0.9/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/CMakeLists.txt` & `pyaogmaneo-2.0.9/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 2e50df8cd14b68438cfb85acdbf3ec2496101034
+        GIT_TAG 762fe2dc916bb9f5a491529af3ba31640fdcd65d
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.8/LICENSE.md` & `pyaogmaneo-2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/PKG-INFO` & `pyaogmaneo-2.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.8/README.md` & `pyaogmaneo-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.0.9/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.8/setup.py` & `pyaogmaneo-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.8",
+    version="2.0.9",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.8/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.0.9/source/pyaogmaneo/py_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         .def_readwrite("down_radius", &pyaon::Layer_Desc::down_radius)
         .def_readwrite("ticks_per_update", &pyaon::Layer_Desc::ticks_per_update)
         .def_readwrite("temporal_horizon", &pyaon::Layer_Desc::temporal_horizon);
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
+        .def_readwrite("code_iters", &aon::Encoder::Params::code_iters)
         .def_readwrite("lr", &aon::Encoder::Params::lr)
         .def_readwrite("gcurve", &aon::Encoder::Params::gcurve);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
         .def_readwrite("lr", &aon::Decoder::Params::lr)
         .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
```

