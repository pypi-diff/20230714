# Comparing `tmp/ahoy_dtu_webthing-0.1.6.tar.gz` & `tmp/ahoy_dtu_webthing-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.1.6.tar", last modified: Wed Jun 28 04:49:44 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-1.0.0.tar", last modified: Fri Jul 14 16:22:11 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.1.6.tar` & `ahoy_dtu_webthing-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:49:44.045973 ahoy_dtu_webthing-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-28 04:49:44.045973 ahoy_dtu_webthing-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:49:44.045973 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 04:49:44.045973 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-28 04:49:44.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-28 04:49:44.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 04:49:44.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-28 04:49:44.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-28 04:49:44.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-28 04:49:44.000000 ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-28 04:49:32.000000 ahoy_dtu_webthing-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-28 04:49:44.045973 ahoy_dtu_webthing-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:22:11.000000 ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 16:21:58.000000 ahoy_dtu_webthing-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:22:11.696062 ahoy_dtu_webthing-1.0.0/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.1.6/LICENSE` & `ahoy_dtu_webthing-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.6/PKG-INFO` & `ahoy_dtu_webthing-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.1.6
+Version: 1.0.0
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.1.6/README.md` & `ahoy_dtu_webthing-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,48 +42,49 @@
         self.listener = None
         Thread(target=self.__periodic_refresh, daemon=True).start()
 
     def close(self):
         self.is_running = False
 
     def __periodic_refresh(self):
-        sleep(randint(0,self.interval))
         while self.is_running:
             try:
+                sleep(randint(0, self.interval))
                 self.refresh()
+                sleep(int(self.interval/2))
             except Exception as e:
                 logging.warning("error occurred refreshing inverter " + self.name + " " + str(e) + " (max " + str(self.power_max) + " watt)")
-            sleep(int(self.interval/2))
+                sleep(5)
 
     def refresh(self):
         # fetch inverter info
-        response = requests.get(self.index_uri)
+        response = requests.get(self.index_uri, timeout=60)
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
-            response = requests.get(self.config_uri)
+            response = requests.get(self.config_uri, timeout=60)
             inverter_configs = response.json()['inverter']
 
             # fetch inverter info
-            response = requests.get(self.inverter_uri)
+            response = requests.get(self.inverter_uri, timeout=60)
             inverter_infos = response.json()['inverter']
 
             # fetch temp, power, etc
-            response = requests.get(self.uri)
+            response = requests.get(self.uri, timeout=60)
             inverter_measures = response.json()['inverter']
 
             p_ac = 0
             i_ac = 0
             u_ac  =0
             p_dc = 0
             p_dc1 = None
```

### Comparing `ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.1.6/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-1.0.0/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.1.6
+Version: 1.0.0
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

