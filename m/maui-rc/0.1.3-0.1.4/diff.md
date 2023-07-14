# Comparing `tmp/maui_rc-0.1.3.tar.gz` & `tmp/maui_rc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maui_rc-0.1.3.tar", max compression
+gzip compressed data, was "maui_rc-0.1.4.tar", max compression
```

## Comparing `maui_rc-0.1.3.tar` & `maui_rc-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.3/LICENSE
--rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.3/maui_rc/__init__.py
--rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.3/maui_rc/datatypes.py
--rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.3/maui_rc/scope.py
--rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.3/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
--rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.3/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
--rw-r--r--   0        0        0     5748 2023-07-14 18:50:36.992217 maui_rc-0.1.3/maui_rc/subsystems/acquisition.py
--rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.3/maui_rc/subsystems/panelsetup.py
--rw-r--r--   0        0        0    20789 2023-07-14 19:11:56.321281 maui_rc-0.1.3/maui_rc/subsystems/wavedata.py
--rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.3/maui_rc/subsystems/waveform.py
--rw-r--r--   0        0        0      555 2023-07-14 19:13:34.132554 maui_rc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.4/LICENSE
+-rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.4/maui_rc/__init__.py
+-rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.4/maui_rc/datatypes.py
+-rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.4/maui_rc/scope.py
+-rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.4/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
+-rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.4/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
+-rw-r--r--   0        0        0     5748 2023-07-14 18:50:36.992217 maui_rc-0.1.4/maui_rc/subsystems/acquisition.py
+-rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.4/maui_rc/subsystems/panelsetup.py
+-rw-r--r--   0        0        0    20905 2023-07-14 19:18:00.821261 maui_rc-0.1.4/maui_rc/subsystems/wavedata.py
+-rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.4/maui_rc/subsystems/waveform.py
+-rw-r--r--   0        0        0      555 2023-07-14 19:18:41.893429 maui_rc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.4/PKG-INFO
```

### Comparing `maui_rc-0.1.3/LICENSE` & `maui_rc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/datatypes.py` & `maui_rc-0.1.4/maui_rc/datatypes.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/scope.py` & `maui_rc-0.1.4/maui_rc/scope.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc` & `maui_rc-0.1.4/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc` & `maui_rc-0.1.4/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/subsystems/acquisition.py` & `maui_rc-0.1.4/maui_rc/subsystems/acquisition.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/subsystems/panelsetup.py` & `maui_rc-0.1.4/maui_rc/subsystems/panelsetup.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/maui_rc/subsystems/wavedata.py` & `maui_rc-0.1.4/maui_rc/subsystems/wavedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,16 @@
 
         return self.Timestamp(year, month, day, hour, minute, second)
 
 
 
     def __parse_to_int(self, data: bytes):
         """Parse a chunk of bytes into an integer."""
+        if len(data) == 1:
+            return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}b", data)[0]
         if len(data) == 2:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}h", data)[0]
         elif len(data) == 4:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}l", data)[0]
         elif len(data) == 8:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}q", data)[0]
         else:
```

### Comparing `maui_rc-0.1.3/maui_rc/subsystems/waveform.py` & `maui_rc-0.1.4/maui_rc/subsystems/waveform.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.3/pyproject.toml` & `maui_rc-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maui-rc"
-version = "0.1.3"
+version = "0.1.4"
 description = "Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes."
 authors = ["Kristofer Karam <karamrkristofer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "maui_rc"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `maui_rc-0.1.3/PKG-INFO` & `maui_rc-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maui-rc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes.
 Author: Kristofer Karam
 Author-email: karamrkristofer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.7.0,<24.0.0)
```

