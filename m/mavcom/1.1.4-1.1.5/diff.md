# Comparing `tmp/mavcom-1.1.4.tar.gz` & `tmp/mavcom-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavcom-1.1.4.tar", last modified: Fri Jul  7 14:26:11 2023, max compression
+gzip compressed data, was "mavcom-1.1.5.tar", last modified: Fri Jul 14 14:27:38 2023, max compression
```

## Comparing `mavcom-1.1.4.tar` & `mavcom-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.488798 mavcom-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 14:25:56.000000 mavcom-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 14:26:11.488798 mavcom-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 14:25:56.000000 mavcom-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 14:25:56.000000 mavcom-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:26:11.488798 mavcom-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.480798 mavcom-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.484798 mavcom-1.1.4/src/mavcom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/loracon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/mavconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/mavcontrol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.484798 mavcom-1.1.4/src/mavcom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.488798 mavcom-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 14:25:56.000000 mavcom-1.1.4/tests/test_mavcom.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-07-14 14:27:38.937303 mavcom-1.1.5/
+-rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.1.5/LICENSE
+-rw-rw-r--   0 main      (1000) main      (1000)     2674 2023-07-14 14:27:38.937303 mavcom-1.1.5/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      848 2023-07-14 14:16:54.000000 mavcom-1.1.5/README.md
+-rw-rw-r--   0 main      (1000) main      (1000)      882 2023-07-14 14:19:24.000000 mavcom-1.1.5/pyproject.toml
+-rw-rw-r--   0 main      (1000) main      (1000)       38 2023-07-14 14:27:38.937303 mavcom-1.1.5/setup.cfg
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-07-14 14:27:38.937303 mavcom-1.1.5/src/
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-07-14 14:27:38.937303 mavcom-1.1.5/src/mavcom/
+-rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.1.5/src/mavcom/__init__.py
+-rw-rw-r--   0 main      (1000) main      (1000)    10534 2023-07-07 14:22:24.000000 mavcom-1.1.5/src/mavcom/loracon.py
+-rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.1.5/src/mavcom/mavconstants.py
+-rw-rw-r--   0 main      (1000) main      (1000)    14010 2023-07-14 14:16:54.000000 mavcom-1.1.5/src/mavcom/mavcontrol.py
+-rw-rw-r--   0 main      (1000) main      (1000)     4544 2023-07-07 14:22:24.000000 mavcom-1.1.5/src/mavcom/video.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-07-14 14:27:38.937303 mavcom-1.1.5/src/mavcom.egg-info/
+-rw-rw-r--   0 main      (1000) main      (1000)     2674 2023-07-14 14:27:38.000000 mavcom-1.1.5/src/mavcom.egg-info/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      376 2023-07-14 14:27:38.000000 mavcom-1.1.5/src/mavcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        1 2023-07-14 14:27:38.000000 mavcom-1.1.5/src/mavcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       52 2023-07-14 14:27:38.000000 mavcom-1.1.5/src/mavcom.egg-info/entry_points.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       49 2023-07-14 14:27:38.000000 mavcom-1.1.5/src/mavcom.egg-info/requires.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        7 2023-07-14 14:27:38.000000 mavcom-1.1.5/src/mavcom.egg-info/top_level.txt
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-07-14 14:27:38.937303 mavcom-1.1.5/tests/
+-rw-rw-r--   0 main      (1000) main      (1000)     1895 2023-07-14 14:16:54.000000 mavcom-1.1.5/tests/test_mavcom.py
```

### Comparing `mavcom-1.1.4/LICENSE` & `mavcom-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.4/PKG-INFO` & `mavcom-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,26 +43,26 @@
 
 ## Installation
 
 ```pip install mavcom```
 
 ## Basic Usage
 
-This is an example of how to use Mavcom with a simulated vehicle.
+This is an example of how to use Mavcom with a simulated vehicle. To connect to a flight controller, you will most likely use UART0, therefore the connection path will instead be "/dev/ttyS0".
 
 Run SITL:
 
 ```sim_vehicle.py -v ArduCopter```
 
 ```python
-from mavcom import mavcontrol
+from mavcom.mavcontrol import Mavcom
 import time
 
-vehicle = mavcom.Mavcom(
-    connection_path = "127.0.0.1:14551",
+vehicle = Mavcom(
+    connection_path = "127.0.0.1:14550",
 )
 
 vehicle.start()
 
 while not vehicle.ready:
     print("Waiting for vehicle to initialise...")
     time.sleep(1)
```

### Comparing `mavcom-1.1.4/README.md` & `mavcom-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 ## Installation
 
 ```pip install mavcom```
 
 ## Basic Usage
 
-This is an example of how to use Mavcom with a simulated vehicle.
+This is an example of how to use Mavcom with a simulated vehicle. To connect to a flight controller, you will most likely use UART0, therefore the connection path will instead be "/dev/ttyS0".
 
 Run SITL:
 
 ```sim_vehicle.py -v ArduCopter```
 
 ```python
-from mavcom import mavcontrol
+from mavcom.mavcontrol import Mavcom
 import time
 
-vehicle = mavcom.Mavcom(
-    connection_path = "127.0.0.1:14551",
+vehicle = Mavcom(
+    connection_path = "127.0.0.1:14550",
 )
 
 vehicle.start()
 
 while not vehicle.ready:
     print("Waiting for vehicle to initialise...")
     time.sleep(1)
```

### Comparing `mavcom-1.1.4/pyproject.toml` & `mavcom-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mavcom"
-version = "1.1.4"
+version = "1.1.5"
 description = "A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers"
 readme = "README.md"
 authors = [{ name = "Mavscient", email = "mavscient@xee4c.33mail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mavcom-1.1.4/src/mavcom/loracon.py` & `mavcom-1.1.5/src/mavcom/loracon.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.4/src/mavcom/mavconstants.py` & `mavcom-1.1.5/src/mavcom/mavconstants.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.4/src/mavcom/mavcontrol.py` & `mavcom-1.1.5/src/mavcom/mavcontrol.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         mandatory_message_types = [
             "HEARTBEAT",
             "GLOBAL_POSITION_INT",
             "GPS_STATUS",
             "GPS_RAW_INT",
             "EKF_STATUS_REPORT",
             "VFR_HUD",
-            "HOME_POSITION"
+            "HOME_POSITION",
+            "SYS_STATUS",
         ]
         self.required_message_types = required_message_types + [m for m in mandatory_message_types if m not in required_message_types]
         self.current_values = defaultdict(lambda: None)
         self.controller = controller
         has_controller = True if controller else False
         
         self._flight_mode = None
@@ -286,22 +287,22 @@
         """
         if "GPS_RAW_INT" not in self.current_values:
             return "GPS not initialised"
         navdata = {
             "eph": self.current_values['GPS_RAW_INT']['eph'],
             "epv": self.current_values['GPS_RAW_INT']['epv'],
             "fix_type": self.current_values['GPS_RAW_INT']['fix_type'],
-            "satellites_visible": self.current_values['GPS_RAW_INT']['satellites_visible']
+            "satellites_visible": self.current_values['GPS_RAW_INT']['satellites_visible'],
         }
         return NavState(navdata['eph'], navdata['epv'], navdata['fix_type'], navdata['satellites_visible'])
     
     @property
-    def vehicle_state(self):
+    def motion_state(self):
         """
-        The current travel state of the vehicle.
+        The current position & motion state of the vehicle.
 
         Attributes
         ----------
         
         - `alt`: altitude AGL relative to home position
         
         - `groundspeed`: groundspeed in m/s
@@ -316,15 +317,34 @@
         """
         alt = self.current_values['GLOBAL_POSITION_INT']['relative_alt'] / 1000
         groundspeed = self.current_values["VFR_HUD"]['groundspeed']
         vertical_speed = self.current_values['VFR_HUD']['climb']
         heading = self.current_values['GLOBAL_POSITION_INT']['hdg']
         lat = self.current_values['GLOBAL_POSITION_INT']['lat'] / 1e7
         lon = self.current_values['GLOBAL_POSITION_INT']['lon'] / 1e7
-        return VehicleState(alt=alt, groundspeed=groundspeed, vertical_speed=vertical_speed, heading=heading, lat=lat, lon=lon)
+        return MotionState(alt=alt, groundspeed=groundspeed, vertical_speed=vertical_speed, heading=heading, lat=lat, lon=lon)
+    
+    @property
+    def battery_state(self):
+        """
+        The current state of the battery.
+
+        Attributes
+        ----------
+        
+        - `voltage`: battery voltage in volts
+        
+        - `current`: battery current in amps
+        
+        - `remaining`: remaining battery percentage
+        """
+        voltage = self.current_values['SYS_STATUS']['voltage_battery'] / 1000
+        current = self.current_values['SYS_STATUS']['current_battery'] / 100
+        remaining = self.current_values['SYS_STATUS']['battery_remaining']
+        return BatteryState(voltage=voltage, current=current, remaining=remaining)
     
 class NavState(object):
     
     def __init__(self, eph, epv, fix_type, satellites_visible) -> None:
         self.eph = eph
         self.epv = epv
         self.fix_type = fix_type
@@ -334,23 +354,40 @@
         return {
             "eph": self.eph,
             "epv": self.epv,
             "fix_type": self.fix_type,
             "satellites_visible": self.satellites_visible
         }
         
-class VehicleState(object):
+class MotionState(object):
     
     def __init__(self, alt, groundspeed, vertical_speed, heading, lat, lon) -> None:
         self.alt = alt
         self.groundspeed = groundspeed
         self.vertical_speed = vertical_speed
         self.heading = heading
         self.lat = lat
         self.lon = lon
     
 class ModeError(Exception):
     def __init__(self, value) -> None:
         self.value = value
         
     def __str__(self):
-        return(repr(self.value))
+        return(repr(self.value))
+    
+class BatteryState(object):
+    """
+    The current state of the battery.
+    
+    Attributes
+    ----------
+    
+    - `voltage`: voltage in millivolts
+    - `current`: current in centiamps
+    - `remaining`: list of cell voltages in millivolts
+    """
+    def __init__(self, voltage, current, remaining) -> None:
+        self.voltage = voltage
+        self.current = current
+        self.remaining = remaining
+        return super().__init__()
```

### Comparing `mavcom-1.1.4/src/mavcom/video.py` & `mavcom-1.1.5/src/mavcom/video.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.4/src/mavcom.egg-info/PKG-INFO` & `mavcom-1.1.5/src/mavcom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,26 +43,26 @@
 
 ## Installation
 
 ```pip install mavcom```
 
 ## Basic Usage
 
-This is an example of how to use Mavcom with a simulated vehicle.
+This is an example of how to use Mavcom with a simulated vehicle. To connect to a flight controller, you will most likely use UART0, therefore the connection path will instead be "/dev/ttyS0".
 
 Run SITL:
 
 ```sim_vehicle.py -v ArduCopter```
 
 ```python
-from mavcom import mavcontrol
+from mavcom.mavcontrol import Mavcom
 import time
 
-vehicle = mavcom.Mavcom(
-    connection_path = "127.0.0.1:14551",
+vehicle = Mavcom(
+    connection_path = "127.0.0.1:14550",
 )
 
 vehicle.start()
 
 while not vehicle.ready:
     print("Waiting for vehicle to initialise...")
     time.sleep(1)
```

