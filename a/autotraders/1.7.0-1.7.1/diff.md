# Comparing `tmp/autotraders-1.7.0.tar.gz` & `tmp/autotraders-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.7.0.tar", last modified: Fri Jul 14 00:36:50 2023, max compression
+gzip compressed data, was "autotraders-1.7.1.tar", last modified: Fri Jul 14 00:49:06 2023, max compression
```

## Comparing `autotraders-1.7.0.tar` & `autotraders-1.7.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.459641 autotraders-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 00:36:36.000000 autotraders-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-14 00:36:50.459641 autotraders-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-14 00:36:36.000000 autotraders-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.451641 autotraders-1.7.0/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/ship_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.451641 autotraders-1.7.0/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 00:36:36.000000 autotraders-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:36:50.459641 autotraders-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.459641 autotraders-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.462068 autotraders-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 00:48:49.000000 autotraders-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-14 00:49:06.462068 autotraders-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-14 00:48:49.000000 autotraders-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.454068 autotraders-1.7.1/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.454068 autotraders-1.7.1/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.458068 autotraders-1.7.1/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.458068 autotraders-1.7.1/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.458068 autotraders-1.7.1/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/shared_models/ship_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.458068 autotraders-1.7.1/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 00:48:49.000000 autotraders-1.7.1/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.454068 autotraders-1.7.1/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-14 00:49:06.000000 autotraders-1.7.1/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 00:49:06.000000 autotraders-1.7.1/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:49:06.000000 autotraders-1.7.1/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 00:49:06.000000 autotraders-1.7.1/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 00:49:06.000000 autotraders-1.7.1/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 00:48:49.000000 autotraders-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:49:06.462068 autotraders-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:49:06.462068 autotraders-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-14 00:48:49.000000 autotraders-1.7.1/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 00:48:49.000000 autotraders-1.7.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-14 00:48:49.000000 autotraders-1.7.1/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-14 00:48:49.000000 autotraders-1.7.1/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-14 00:48:49.000000 autotraders-1.7.1/tests/test_util.py
```

### Comparing `autotraders-1.7.0/LICENSE` & `autotraders-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/PKG-INFO` & `autotraders-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.7.0
+Version: 1.7.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://comsictraders.github.io/autotraders/
 Project-URL: Repository, https://github.com/comsictraders/autotraders.git
 Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://comsictraders.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
```

### Comparing `autotraders-1.7.0/README.md` & `autotraders-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/agent.py` & `autotraders-1.7.1/autotraders/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
             self.account_id = data["accountId"]
             self.ships = Ship.all(self.session)
             self.contracts = Contract.all(self.session)
         self.symbol = data["symbol"]
         self.headquarters = MapSymbol(data["headquarters"])
         self.credits = data["credits"]
         self.starting_faction = data["startingFaction"]
-        self.ship_count = data["shipCount"]
+        if "shipCount" in data:
+            self.ship_count = data["shipCount"]
 
     @staticmethod
     def all(session, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
                 + "agents?limit="
```

### Comparing `autotraders-1.7.0/autotraders/faction/__init__.py` & `autotraders-1.7.1/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/faction/contract.py` & `autotraders-1.7.1/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/map/system.py` & `autotraders-1.7.1/autotraders/map/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,7 +56,10 @@
                 systems.append(s)
             return systems, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
+
+    def __hash__(self):
+        return hash(self.symbol)
```

### Comparing `autotraders-1.7.0/autotraders/map/waypoint.py` & `autotraders-1.7.1/autotraders/map/waypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,7 +80,10 @@
                 waypoints.append(waypoint)
             return waypoints, j["meta"]["total"]
 
         return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
+
+    def __hash__(self):
+        return hash(self.symbol)
```

### Comparing `autotraders-1.7.0/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.7.1/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.7.1/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.7.1/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.7.1/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/paginated_list.py` & `autotraders-1.7.1/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/session.py` & `autotraders-1.7.1/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/shared_models/map_symbol.py` & `autotraders-1.7.1/autotraders/shared_models/map_symbol.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.raw = s
 
     def __str__(self):
         """Returns the input that was passed as a string."""
         return self.raw
 
     def __hash__(self):
-        return self.raw
+        return hash(self.raw)
 
     def __add__(self, other):
         return self / other
 
     def __truediv__(self, other):
         """Concatenates with a '-'"""
         assert isinstance(other, str)
```

### Comparing `autotraders-1.7.0/autotraders/shared_models/transaction.py` & `autotraders-1.7.1/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/ship/__init__.py` & `autotraders-1.7.1/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/ship/cargo.py` & `autotraders-1.7.1/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/ship/nav.py` & `autotraders-1.7.1/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/ship/ship_components.py` & `autotraders-1.7.1/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/space_traders_entity.py` & `autotraders-1.7.1/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/status.py` & `autotraders-1.7.1/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders/util.py` & `autotraders-1.7.1/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/autotraders.egg-info/PKG-INFO` & `autotraders-1.7.1/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.7.0
+Version: 1.7.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://comsictraders.github.io/autotraders/
 Project-URL: Repository, https://github.com/comsictraders/autotraders.git
 Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://comsictraders.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
```

### Comparing `autotraders-1.7.0/autotraders.egg-info/SOURCES.txt` & `autotraders-1.7.1/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/pyproject.toml` & `autotraders-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/tests/test_init.py` & `autotraders-1.7.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/tests/test_map.py` & `autotraders-1.7.1/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/tests/test_ship.py` & `autotraders-1.7.1/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.7.0/tests/test_util.py` & `autotraders-1.7.1/tests/test_util.py`

 * *Files identical despite different names*

