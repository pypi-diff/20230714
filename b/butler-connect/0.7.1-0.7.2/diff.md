# Comparing `tmp/butler-connect-0.7.1.tar.gz` & `tmp/butler-connect-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.7.1.tar", last modified: Sat Jul  8 09:44:14 2023, max compression
+gzip compressed data, was "butler-connect-0.7.2.tar", last modified: Fri Jul 14 19:27:03 2023, max compression
```

## Comparing `butler-connect-0.7.1.tar` & `butler-connect-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.232107 butler-connect-0.7.1/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     2584 2023-07-08 09:44:14.231117 butler-connect-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      809 2023-07-08 09:42:59.000000 butler-connect-0.7.1/README.md
--rw-rw-rw-   0        0        0      738 2023-07-08 09:42:21.000000 butler-connect-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 09:44:14.232107 butler-connect-0.7.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.200104 butler-connect-0.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.203167 butler-connect-0.7.1/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.1/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.1/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.213095 butler-connect-0.7.1/src/butlerDescription/
--rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.1/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.1/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.1/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.7.1/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     2034 2023-07-08 09:43:40.000000 butler-connect-0.7.1/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-08 09:44:14.231117 butler-connect-0.7.1/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2584 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-08 09:44:14.000000 butler-connect-0.7.1/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.339659 butler-connect-0.7.2/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     2712 2023-07-14 19:27:03.338657 butler-connect-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2023-07-14 19:26:32.000000 butler-connect-0.7.2/README.md
+-rw-rw-rw-   0        0        0      738 2023-07-14 19:25:40.000000 butler-connect-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 19:27:03.339659 butler-connect-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.304568 butler-connect-0.7.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.307568 butler-connect-0.7.2/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.2/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.2/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.320599 butler-connect-0.7.2/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.2/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.2/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.2/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.7.2/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     2596 2023-07-14 19:26:51.000000 butler-connect-0.7.2/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.337637 butler-connect-0.7.2/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2712 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.7.1/LICENSE` & `butler-connect-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.1/PKG-INFO` & `butler-connect-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.1
+Version: 0.7.2
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,7 +57,11 @@
 - add new signal  types f.ex. system_state or set_temperature.heater
 
 ### 0.7.0
 - change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
 
 ### 0.7.1
 - Bugifx in Signal().__init__(.. ext was missing)
+### 0.7.2
+- create SignalDirection()
+- add convertFrom to SignalOptionType
+- add different consumptionSignals to SignalType
```

### Comparing `butler-connect-0.7.1/README.md` & `butler-connect-0.7.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 ### 0.6.0
 - add new signal  types f.ex. system_state or set_temperature.heater
 
 ### 0.7.0
 - change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
 
 ### 0.7.1
-- Bugifx in Signal().__init__(.. ext was missing)
+- Bugifx in Signal().__init__(.. ext was missing)
+### 0.7.2
+- create SignalDirection()
+- add convertFrom to SignalOptionType
+- add different consumptionSignals to SignalType
```

### Comparing `butler-connect-0.7.1/pyproject.toml` & `butler-connect-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.7.1"
+version = "0.7.2"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.7.1/src/butlerConnect/pikaButler.py` & `butler-connect-0.7.2/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.1/src/butlerDescription/control.py` & `butler-connect-0.7.2/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.1/src/butlerDescription/signal.py` & `butler-connect-0.7.2/src/butlerDescription/signal.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,19 +16,35 @@
     presence_merged = 'presence_merged'
     illumination = 'illumination'
     actuatorValue = 'actuator_value'
     systemState = 'system_state'
     class systemState_():
         heater = 'system_state_heater'
         cooler = 'system_state_cooler'
+    consumptionGas = 'consumption_gas'
+    consumptionGasRel = 'consumption_gas_rel'
+    consumptionPower = 'consumption_power'
+    consumptionPowerRel = 'consumption_power_rel'
+    consumptionWater = 'consumption_water'
+    consumptionWaterRel = 'consumption_water_rel'
+    consumptionHeat = 'consumption_heat'
+    consumptionHeatRel = 'consumption_heat_rel'
+    consumptionCool = 'consumption_cool'
+    consumptionCoolRel = 'consumption_cool_rel'
+    
     
 
 class SignalOptionType():
     unDef = 'undef'
     forwardingMQTT = 'forwarding_mqtt'
+    convertFrom    = 'convert_from'
+    
+class SignalDirection():
+    input = 'input'
+    output = 'output'
     
 
 
 class Signal():
     def __init__(self,type,component=0,group=0,ioDevice="",ioSignal="",parameter={},timestamp=datetime.now(),value = 0.0,valueStr = "",ext={}):
         self.timestamp  = timestamp
         self.component  = int(component)
```

### Comparing `butler-connect-0.7.1/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.7.2/src/butler_connect.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.1
+Version: 0.7.2
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,7 +57,11 @@
 - add new signal  types f.ex. system_state or set_temperature.heater
 
 ### 0.7.0
 - change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
 
 ### 0.7.1
 - Bugifx in Signal().__init__(.. ext was missing)
+### 0.7.2
+- create SignalDirection()
+- add convertFrom to SignalOptionType
+- add different consumptionSignals to SignalType
```

