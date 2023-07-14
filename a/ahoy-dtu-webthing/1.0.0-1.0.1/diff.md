# Comparing `tmp/ahoy_dtu_webthing-1.0.0.tar.gz` & `tmp/ahoy_dtu_webthing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-1.0.0.tar", last modified: Fri Jul 14 16:22:11 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-1.0.1.tar", last modified: Fri Jul 14 16:34:12 2023, max compression
```

## Comparing `ahoy_dtu_webthing-1.0.0.tar` & `ahoy_dtu_webthing-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:34:12.945266 ahoy_dtu_webthing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:34:12.945266 ahoy_dtu_webthing-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:34:12.941266 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:34:12.945266 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:34:12.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 16:34:12.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:34:12.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 16:34:12.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 16:34:12.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:34:12.000000 ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 16:33:54.000000 ahoy_dtu_webthing-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:34:12.945266 ahoy_dtu_webthing-1.0.1/setup.cfg
```

### Comparing `ahoy_dtu_webthing-1.0.0/LICENSE` & `ahoy_dtu_webthing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.0/PKG-INFO` & `ahoy_dtu_webthing-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-1.0.0/README.md` & `ahoy_dtu_webthing-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/dtu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from threading import Thread
 from random import randint
 import re
 import requests
+from requests import Session
 import logging
 from time import sleep
 from datetime import datetime
 
 class Inverter:
 
     def __init__(self, base_uri: str, id: int, channels: int, name: str, serial: str, interval: int):
@@ -42,49 +43,51 @@
         self.listener = None
         Thread(target=self.__periodic_refresh, daemon=True).start()
 
     def close(self):
         self.is_running = False
 
     def __periodic_refresh(self):
+        session = Session()
         while self.is_running:
             try:
                 sleep(randint(0, self.interval))
-                self.refresh()
+                self.refresh(session)
                 sleep(int(self.interval/2))
             except Exception as e:
                 logging.warning("error occurred refreshing inverter " + self.name + " " + str(e) + " (max " + str(self.power_max) + " watt)")
                 sleep(5)
+                session = Session()
 
-    def refresh(self):
+    def refresh(self, session: Session):
         # fetch inverter info
-        response = requests.get(self.index_uri, timeout=60)
+        response = session.get(self.index_uri, timeout=60)
         inverter_state = response.json()['inverter']
 
         previous_is_available = self.is_available
         self.is_available = inverter_state[self.id]['is_avail']
         if previous_is_available != self.is_available:
             logging.info("inverter " + str(self.name) + " is " + ("" if self.is_available else "not ") + "available")
 
         previous_is_producing = self.is_producing
         self.is_producing = inverter_state[self.id]['is_producing']
         if previous_is_producing != self.is_producing:
             logging.info("inverter " + str(self.name) + " is " + ("" if self.is_producing else "not ") + "producing")
 
         if self.is_producing:
             # fetch power limit
-            response = requests.get(self.config_uri, timeout=60)
+            response = session.get(self.config_uri, timeout=60)
             inverter_configs = response.json()['inverter']
 
             # fetch inverter info
-            response = requests.get(self.inverter_uri, timeout=60)
+            response = session.get(self.inverter_uri, timeout=60)
             inverter_infos = response.json()['inverter']
 
             # fetch temp, power, etc
-            response = requests.get(self.uri, timeout=60)
+            response = session.get(self.uri, timeout=60)
             inverter_measures = response.json()['inverter']
 
             p_ac = 0
             i_ac = 0
             u_ac  =0
             p_dc = 0
             p_dc1 = None
@@ -162,15 +165,15 @@
         self.__notify_Listener()
 
     def register_listener(self, listener):
         self.listener = listener
 
     def __notify_Listener(self):
         if self.listener is not None:
-            self.listener()
+            self.listener(self)
 
     def __str__(self):
         return self.name + " " + self.serial + " (P_AC: " + str(self.p_ac) + ", U_AC: " + str(self.u_ac) + ", I_AC: " + str(self.i_ac) + \
                 ", P_DC: " + str(self.p_dc) + ", EFFICIENCY: " + str(self.efficiency) +  ")"
 
     def __repr__(self):
         return  self.__str__()
```

### Comparing `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                          'readOnly': True,
                      }))
 
 
         self.ioloop = tornado.ioloop.IOLoop.current()
         self.inverter.register_listener(self.on_value_changed)
 
-    def on_value_changed(self):
+    def on_value_changed(self, inverter: Inverter):
         self.ioloop.add_callback(self.__on_value_changed)
 
     def __on_value_changed(self):
         self.producing.notify_of_external_update(self.inverter.is_producing)
         self.available.notify_of_external_update(self.inverter.is_available)
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
         self.p_dc1.notify_of_external_update(self.inverter.p_dc1)
```

### Comparing `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-1.0.1/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

