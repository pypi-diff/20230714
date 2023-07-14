# Comparing `tmp/maui_rc-0.1.0.tar.gz` & `tmp/maui_rc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maui_rc-0.1.0.tar", max compression
+gzip compressed data, was "maui_rc-0.1.1.tar", max compression
```

## Comparing `maui_rc-0.1.0.tar` & `maui_rc-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.0/LICENSE
--rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.0/maui_rc/__init__.py
--rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.0/maui_rc/datatypes.py
--rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.0/maui_rc/scope.py
--rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.0/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
--rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.0/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
--rw-r--r--   0        0        0     5691 2023-07-14 16:41:59.774449 maui_rc-0.1.0/maui_rc/subsystems/acquisition.py
--rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.0/maui_rc/subsystems/panelsetup.py
--rw-r--r--   0        0        0    19757 2023-07-14 16:36:38.812473 maui_rc-0.1.0/maui_rc/subsystems/wavedata.py
--rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.0/maui_rc/subsystems/waveform.py
--rw-r--r--   0        0        0      555 2023-07-14 16:15:20.389222 maui_rc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.1/LICENSE
+-rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.1/maui_rc/__init__.py
+-rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.1/maui_rc/datatypes.py
+-rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.1/maui_rc/scope.py
+-rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.1/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
+-rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.1/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
+-rw-r--r--   0        0        0     5851 2023-07-14 17:04:21.070058 maui_rc-0.1.1/maui_rc/subsystems/acquisition.py
+-rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.1/maui_rc/subsystems/panelsetup.py
+-rw-r--r--   0        0        0    19757 2023-07-14 16:36:38.812473 maui_rc-0.1.1/maui_rc/subsystems/wavedata.py
+-rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.1/maui_rc/subsystems/waveform.py
+-rw-r--r--   0        0        0      555 2023-07-14 17:05:49.721542 maui_rc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.1/PKG-INFO
```

### Comparing `maui_rc-0.1.0/LICENSE` & `maui_rc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/datatypes.py` & `maui_rc-0.1.1/maui_rc/datatypes.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/scope.py` & `maui_rc-0.1.1/maui_rc/scope.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc` & `maui_rc-0.1.1/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc` & `maui_rc-0.1.1/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/subsystems/acquisition.py` & `maui_rc-0.1.1/maui_rc/subsystems/acquisition.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,18 +160,23 @@
         mode = TriggerMode(resp)
         return mode
 
     def get_waveform_data(self, channel: Channel) -> tuple[np.array, np.array]:
         """Extract the waveform from the scope and parse it."""
 
         # Transfer the data blocks over
-        desc = self.__scope.query(f"{channel}:WF? DESC")
-        text = self.__scope.query(f"{channel}:WF? TEXT")
-        time = self.__scope.query(f"{channel}:WF? TIME")
-        dat1 = self.__scope.query(f"{channel}:WF? DAT1")
-        dat2 = self.__scope.query(f"{channel}:WF? DAT2")
+        self.__scope.write(f"{channel}:WF? DESC")
+        desc = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? TEXT")
+        text = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? TIME")
+        time = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? DAT1")
+        dat1 = self.__scope.read_raw()
+        self.__scope.write(f"{channel}:WF? DAT2")
+        dat2 = self.__scope.read_raw()
 
         # Parse it into waveform data
         data = WaveformData(desc, text, time, dat1, dat2)
 
         # Return a tuple of arrays (x,y)
         return (data.data_x, data.data_y)
```

### Comparing `maui_rc-0.1.0/maui_rc/subsystems/panelsetup.py` & `maui_rc-0.1.1/maui_rc/subsystems/panelsetup.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/subsystems/wavedata.py` & `maui_rc-0.1.1/maui_rc/subsystems/wavedata.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/maui_rc/subsystems/waveform.py` & `maui_rc-0.1.1/maui_rc/subsystems/waveform.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.0/pyproject.toml` & `maui_rc-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maui-rc"
-version = "0.1.0"
+version = "0.1.1"
 description = "Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes."
 authors = ["Kristofer Karam <karamrkristofer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "maui_rc"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `maui_rc-0.1.0/PKG-INFO` & `maui_rc-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maui-rc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes.
 Author: Kristofer Karam
 Author-email: karamrkristofer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.7.0,<24.0.0)
```

