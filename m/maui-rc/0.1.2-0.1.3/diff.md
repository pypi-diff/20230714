# Comparing `tmp/maui_rc-0.1.2.tar.gz` & `tmp/maui_rc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maui_rc-0.1.2.tar", max compression
+gzip compressed data, was "maui_rc-0.1.3.tar", max compression
```

## Comparing `maui_rc-0.1.2.tar` & `maui_rc-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.2/LICENSE
--rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.2/maui_rc/__init__.py
--rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.2/maui_rc/datatypes.py
--rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.2/maui_rc/scope.py
--rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.2/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
--rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.2/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
--rw-r--r--   0        0        0     5748 2023-07-14 18:50:36.992217 maui_rc-0.1.2/maui_rc/subsystems/acquisition.py
--rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.2/maui_rc/subsystems/panelsetup.py
--rw-r--r--   0        0        0    19757 2023-07-14 16:36:38.812473 maui_rc-0.1.2/maui_rc/subsystems/wavedata.py
--rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.2/maui_rc/subsystems/waveform.py
--rw-r--r--   0        0        0      555 2023-07-14 18:51:39.584137 maui_rc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 18:57:19.313033 maui_rc-0.1.3/LICENSE
+-rw-r--r--   0        0        0      428 2023-07-14 16:21:55.690359 maui_rc-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 17:59:16.563721 maui_rc-0.1.3/maui_rc/__init__.py
+-rw-r--r--   0        0        0     1465 2023-07-12 18:25:18.798902 maui_rc-0.1.3/maui_rc/datatypes.py
+-rw-r--r--   0        0        0     2162 2023-07-14 13:56:51.341351 maui_rc-0.1.3/maui_rc/scope.py
+-rw-r--r--   0        0        0     8370 2023-07-12 18:25:22.685593 maui_rc-0.1.3/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc
+-rw-r--r--   0        0        0     1998 2023-07-14 13:35:18.849347 maui_rc-0.1.3/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc
+-rw-r--r--   0        0        0     5748 2023-07-14 18:50:36.992217 maui_rc-0.1.3/maui_rc/subsystems/acquisition.py
+-rw-r--r--   0        0        0     1105 2023-07-12 18:50:16.865554 maui_rc-0.1.3/maui_rc/subsystems/panelsetup.py
+-rw-r--r--   0        0        0    20789 2023-07-14 19:11:56.321281 maui_rc-0.1.3/maui_rc/subsystems/wavedata.py
+-rw-r--r--   0        0        0     2727 2023-07-14 15:45:28.430242 maui_rc-0.1.3/maui_rc/subsystems/waveform.py
+-rw-r--r--   0        0        0      555 2023-07-14 19:13:34.132554 maui_rc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 maui_rc-0.1.3/PKG-INFO
```

### Comparing `maui_rc-0.1.2/LICENSE` & `maui_rc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/datatypes.py` & `maui_rc-0.1.3/maui_rc/datatypes.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/scope.py` & `maui_rc-0.1.3/maui_rc/scope.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc` & `maui_rc-0.1.3/maui_rc/subsystems/__pycache__/acquisition.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc` & `maui_rc-0.1.3/maui_rc/subsystems/__pycache__/panelsetup.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/subsystems/acquisition.py` & `maui_rc-0.1.3/maui_rc/subsystems/acquisition.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/subsystems/panelsetup.py` & `maui_rc-0.1.3/maui_rc/subsystems/panelsetup.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/maui_rc/subsystems/wavedata.py` & `maui_rc-0.1.3/maui_rc/subsystems/wavedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
 import struct
 import numpy as np
 
-
 class WaveformData:
 
     class RecordType(Enum):
         SingleSweep = 0
         Interleaved = 1
         Histogram = 2
         Graph = 3
@@ -169,14 +168,26 @@
         CHANNEL_3 = 2
         CHANNEL_4 = 3
         UNKNOWN = 9
 
         def __str__(self):
             return self.name
         
+    class Timestamp:
+        def __init__(self, year: int, month: int, day: int, hour: int, minute: int, second: float):
+            self.year = year
+            self.month = month
+            self.day = day
+            self.hour = hour
+            self.minute = minute
+            self.second = second
+
+        def __str__(self):
+            return f"{self.year}-{self.month}-{self.day} {self.hour}:{self.minute}:{self.second}"
+
     # GENERAL DESCRIPTION VARIABLES
 
     byteorder: str
     """Order in which bytes are read to numbers in the waveform data"""
     wf_datapoint_size: int
     """Size in bytes of a single data point in the waveform data"""
 
@@ -259,18 +270,17 @@
     pixel_offset: float
     """Needed to know how to display the waveform."""
 
     vertical_unit: str
     """Units of the vertical axis."""
     horizontal_unit: str
     """Units of the horizontal axis."""
-
     horizontal_uncertainty: float
     """Uncertainty from one acquisition to the next, of the horizontal offset in seconds"""
-    trigger_time: float
+    trigger_time: Timestamp
     """Time of the trigger."""
     acquisition_duration: float
     """Duration of the acquisition in seconds."""
 
     record_type: RecordType
     """What kind of data we was transfered. Defines how we will treat it."""
     processing_done: ProcessingDone
@@ -298,14 +308,30 @@
     wave_source: Source
     """The channel from which the data comes from."""
 
     def __parse_to_string(self, data: bytes):
         """Parse a chunk of bytes into a string."""
         return data.decode('utf-8').strip("\x00").strip()
     
+    def __parse_timestamp(self, data: bytes):
+        """Parse a chunk of bytes as a timestamp"""
+        if len(data) != 16:
+            raise Exception("parsing error: timestamp must be 16 bytes long")
+        
+        second = self.__parse_to_float(data[0:8])
+        minute = self.__parse_to_int(data[8:9])
+        hour = self.__parse_to_int(data[9:10])
+        day = self.__parse_to_int(data[10:11])
+        month = self.__parse_to_int(data[11:12])
+        year = self.__parse_to_int(data[12:14])
+
+        return self.Timestamp(year, month, day, hour, minute, second)
+
+
+
     def __parse_to_int(self, data: bytes):
         """Parse a chunk of bytes into an integer."""
         if len(data) == 2:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}h", data)[0]
         elif len(data) == 4:
             return struct.unpack(f"{'>' if self.byteorder == 'big' else '<'}l", data)[0]
         elif len(data) == 8:
@@ -396,15 +422,15 @@
         self.nominal_subarray_count = self.__parse_to_int(desc[174:176])
         self.horizontal_interval = self.__parse_to_float(desc[176:180])
         self.horizontal_offset = self.__parse_to_float(desc[180:188])
         self.pixel_offset = self.__parse_to_float(desc[188:196])
         self.vertical_unit = desc[196:244]
         self.horizontal_unit = desc[244:292]
         self.horizontal_uncertainty = self.__parse_to_float(desc[292:296])
-        self.trigger_time = desc[296:312]
+        self.trigger_time = self.__parse_timestamp(desc[296:312])
         self.acquisition_duration = self.__parse_to_float(desc[312:316])
         self.record_type = self.RecordType(self.__parse_to_int(desc[316:318]))
         self.processing_done = self.ProcessingDone(self.__parse_to_int(desc[318:320]))
         self.ris_sweeps = self.__parse_to_int(desc[322:324])
         self.timebase = self.TimeBase(self.__parse_to_int(desc[324:326]))
         self.vertical_coupling = self.Coupling(self.__parse_to_int(desc[326:328]))
         self.probe_attenuation = self.__parse_to_float(desc[328:332])
```

### Comparing `maui_rc-0.1.2/maui_rc/subsystems/waveform.py` & `maui_rc-0.1.3/maui_rc/subsystems/waveform.py`

 * *Files identical despite different names*

### Comparing `maui_rc-0.1.2/pyproject.toml` & `maui_rc-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maui-rc"
-version = "0.1.2"
+version = "0.1.3"
 description = "Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes."
 authors = ["Kristofer Karam <karamrkristofer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "maui_rc"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `maui_rc-0.1.2/PKG-INFO` & `maui_rc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maui-rc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper for controlling Teledyne-Lecroy Maui oscilloscopes.
 Author: Kristofer Karam
 Author-email: karamrkristofer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.7.0,<24.0.0)
```

