# Comparing `tmp/ahoy_dtu_webthing-1.0.2.tar.gz` & `tmp/ahoy_dtu_webthing-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-1.0.2.tar", last modified: Fri Jul 14 16:37:27 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-1.0.3.tar", last modified: Fri Jul 14 16:44:48 2023, max compression
```

## Comparing `ahoy_dtu_webthing-1.0.2.tar` & `ahoy_dtu_webthing-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:37:27.506777 ahoy_dtu_webthing-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:37:27.506777 ahoy_dtu_webthing-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:37:27.506777 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:37:27.506777 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:37:27.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 16:37:27.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:37:27.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 16:37:27.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 16:37:27.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:37:27.000000 ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 16:37:06.000000 ahoy_dtu_webthing-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:37:27.506777 ahoy_dtu_webthing-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:44:48.580673 ahoy_dtu_webthing-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:44:48.580673 ahoy_dtu_webthing-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:44:48.576673 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:44:48.580673 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:44:48.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 16:44:48.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:44:48.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 16:44:48.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 16:44:48.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:44:48.000000 ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 16:44:30.000000 ahoy_dtu_webthing-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:44:48.580673 ahoy_dtu_webthing-1.0.3/setup.cfg
```

### Comparing `ahoy_dtu_webthing-1.0.2/LICENSE` & `ahoy_dtu_webthing-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.2/PKG-INFO` & `ahoy_dtu_webthing-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-1.0.2/README.md` & `ahoy_dtu_webthing-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/dtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,57 +38,67 @@
         self.efficiency = 0
         self.power_max = 0
         self.power_limit = 0
         self.last_update = datetime.fromtimestamp(0)
         self.is_available = False
         self.is_producing = False
         self.listener = None
+        self.session = Session()
         Thread(target=self.__periodic_refresh, daemon=True).start()
 
     def close(self):
         self.is_running = False
 
+    def __renew_session(self):
+        try:
+            self.session.close()
+        except Exception as e:
+            logging.warning("error occurred closing session " + str(e))
+        self.session = Session()
+
     def __periodic_refresh(self):
-        session = Session()
         while self.is_running:
             try:
                 sleep(randint(0, self.interval))
-                self.refresh(session)
+                self.refresh()
                 sleep(int(self.interval/2))
             except Exception as e:
                 logging.warning("error occurred refreshing inverter " + self.name + " " + str(e) + " (max " + str(self.power_max) + " watt)")
                 sleep(5)
-                session = Session()
+                try:
+                    self.__renew_session()
+                except Exception as e:
+                    logging.warning("error occurred renewing session " + str(e))
 
-    def refresh(self, session: Session):
+    def refresh(self):
         # fetch inverter info
-        response = session.get(self.index_uri, timeout=60)
+        response = self.session.get(self.index_uri, timeout=60)
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
-            response = session.get(self.config_uri, timeout=60)
+            response = self.session.get(self.config_uri, timeout=60)
             inverter_configs = response.json()['inverter']
 
             # fetch inverter info
-            response = session.get(self.inverter_uri, timeout=60)
+            response = self.session.get(self.inverter_uri, timeout=60)
             inverter_infos = response.json()['inverter']
 
             # fetch temp, power, etc
-            response = session.get(self.live_uri, timeout=60)
+            response = self.session.get(self.live_uri, timeout=60)
             inverter_measures = response.json()['inverter']
 
             p_ac = 0
             i_ac = 0
             u_ac  =0
             p_dc = 0
             p_dc1 = None
@@ -138,14 +148,15 @@
                     temp = float(measure['val'])
                 elif measure['fld'] == 'F_AC':
                     frequency = float(measure['val'])
 
             self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, p_dc1, p_dc2, u_dc1, u_dc2, i_dc1, i_dc2, efficiency, temp, frequency)
         else:
             self.update(self.power_max, self.power_limit, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0)
+
     def set_power_limit(self, limit_watt: int):
         logging.info("inverter " + self.name + " set power limit to " + str(limit_watt) + " watt")
         requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
 
     def update(self, power_max: int, power_limit: int, p_ac: float, u_ac: float, i_ac: float, p_dc: float, p_dc1:float, p_dc2: float, u_dc1: float, u_dc2: float, i_dc1: float, i_dc2: float, efficiency: float, temp: float, frequency: float):
         self.power_max = power_max
         self.power_limit = power_limit
```

### Comparing `ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-1.0.2/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-1.0.3/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

