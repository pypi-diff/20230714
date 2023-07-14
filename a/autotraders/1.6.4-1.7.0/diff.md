# Comparing `tmp/autotraders-1.6.4.tar.gz` & `tmp/autotraders-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.6.4.tar", last modified: Sat Jul  8 22:53:35 2023, max compression
+gzip compressed data, was "autotraders-1.7.0.tar", last modified: Fri Jul 14 00:36:50 2023, max compression
```

## Comparing `autotraders-1.6.4.tar` & `autotraders-1.7.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.264073 autotraders-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:53:23.000000 autotraders-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:53:35.264073 autotraders-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-08 22:53:23.000000 autotraders-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/ship_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 22:53:23.000000 autotraders-1.6.4/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.260073 autotraders-1.6.4/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 22:53:35.000000 autotraders-1.6.4/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-08 22:53:23.000000 autotraders-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:53:35.264073 autotraders-1.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:35.264073 autotraders-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 22:53:23.000000 autotraders-1.6.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.459641 autotraders-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 00:36:36.000000 autotraders-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-14 00:36:50.459641 autotraders-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-14 00:36:36.000000 autotraders-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.451641 autotraders-1.7.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/ship_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.455641 autotraders-1.7.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 00:36:36.000000 autotraders-1.7.0/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.451641 autotraders-1.7.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 00:36:50.000000 autotraders-1.7.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 00:36:36.000000 autotraders-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:36:50.459641 autotraders-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:36:50.459641 autotraders-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-14 00:36:36.000000 autotraders-1.7.0/tests/test_util.py
```

### Comparing `autotraders-1.6.4/LICENSE` & `autotraders-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/PKG-INFO` & `autotraders-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.4
+Version: 1.7.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://comsictraders.github.io/autotraders/
 Project-URL: Repository, https://github.com/comsictraders/autotraders.git
 Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://comsictraders.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
```

### Comparing `autotraders-1.6.4/README.md` & `autotraders-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/agent.py` & `autotraders-1.7.0/autotraders/map/waypoint_types/shipyard.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,46 @@
-from autotraders.faction.contract import Contract
-from autotraders.paginated_list import PaginatedList
-from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.space_traders_entity import SpaceTradersEntity
+from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
-from autotraders.ship import Ship
+from autotraders.shared_models.transaction import ShipyardTransaction
+from autotraders.ship import Frame, Reactor, Engine, Module, Mount, Ship
 
 
-class Agent(SpaceTradersEntity):
-    contracts: PaginatedList
-    starting_faction: str
-    symbol: str
-    account_id: str
-    credits: int
-    ships: PaginatedList
-    headquarters: MapSymbol
+class ShipyardShip:
+    def __init__(self, data):
+        self.ship_type = data["type"]
+        self.name = data["name"]
+        self.description = data["description"]
+        self.purchase_price = data["purchasePrice"]
+        self.frame = Frame(data["frame"])
+        self.reactor = Reactor(data["reactor"])
+        self.engine = Engine(data["engine"])
+        self.modules = [Module(d) for d in data["modules"]]
+        self.mounts = [Mount(d) for d in data["mounts"]]
 
-    def __init__(self, session: AutoTradersSession, data=None):
-        super().__init__(session, "my/agent", data)
 
-    def update(self, data=None):
-        """Uses 3 API requests to get all agent details"""
+class Shipyard(WaypointType):
+    ship_types: list[str]
+    ships: list[ShipyardShip]
+
+    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
+        super().__init__(waypoint, "shipyard", session, data)
+
+    def update(self, data: dict = None):
         if data is None:
             data = self.get()["data"]
-        self.account_id = data["accountId"]
-        self.symbol = data["symbol"]
-        self.headquarters = MapSymbol(data["headquarters"])
-        self.credits = data["credits"]
-        self.starting_faction = data["startingFaction"]
-        self.ships = Ship.all(self.session)
-        self.contracts = Contract.all(self.session)
+        self.ship_types = []
+        for ship_type in data["shipTypes"]:
+            self.ship_types.append(ship_type["type"])
+        self.ships = None
+        if "ships" in data:
+            self.ships = []
+            for ship in data["ships"]:
+                self.ships.append(ShipyardShip(ship))
+
+    def purchase(self, ship_type: str):
+        j = self.session.post(
+            self.session.base_url + "my/ships",
+            data={"shipType": ship_type, "waypointSymbol": self.location},
+        ).json()
+        return Ship(
+            j["data"]["ship"]["symbol"], self.session, j["data"]["ship"]
+        ), ShipyardTransaction(j["data"]["transaction"])
```

### Comparing `autotraders-1.6.4/autotraders/faction/__init__.py` & `autotraders-1.7.0/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/faction/contract.py` & `autotraders-1.7.0/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/map/system.py` & `autotraders-1.7.0/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/map/waypoint.py` & `autotraders-1.7.0/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.7.0/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.7.0/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.7.0/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.7.0/autotraders/ship/ship_components.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,66 @@
-from autotraders.map.waypoint_types import WaypointType
-from autotraders.session import AutoTradersSession
-from autotraders.shared_models.transaction import ShipyardTransaction
-from autotraders.ship import Frame, Reactor, Engine, Module, Mount, Ship
+from datetime import datetime
+from typing import Optional
 
 
-class ShipyardShip:
+class Requirements:
     def __init__(self, data):
-        self.ship_type = data["type"]
+        if "power" in data:
+            self.power = data["power"]
+        if "crew" in data:
+            self.crew = data["crew"]
+        if "slots" in data:
+            self.slots = data["slots"]
+
+
+class ShipComponent:
+    def __init__(self, data):
+        self.symbol = data["symbol"]
         self.name = data["name"]
-        self.description = data["description"]
-        self.purchase_price = data["purchasePrice"]
-        self.frame = Frame(data["frame"])
-        self.reactor = Reactor(data["reactor"])
-        self.engine = Engine(data["engine"])
-        self.modules = [Module(d) for d in data["modules"]]
-        self.mounts = [Mount(d) for d in data["mounts"]]
-
-
-class Shipyard(WaypointType):
-    ship_types: list[str]
-    ships: list[ShipyardShip]
-
-    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
-        super().__init__(waypoint, "shipyard", session, data)
-
-    def update(self, data: dict = None):
-        if data is None:
-            data = self.get()["data"]
-        self.ship_types = []
-        for ship_type in data["shipTypes"]:
-            self.ship_types.append(ship_type["type"])
-        self.ships = None
-        if "ships" in data:
-            self.ships = []
-            for ship in data["ships"]:
-                self.ships.append(ShipyardShip(ship))
-
-    def purchase(self, ship_type: str):
-        j = self.session.post(
-            self.session.base_url + "my/ships",
-            data={"shipType": ship_type, "waypointSymbol": self.location},
-        ).json()
-        return Ship(
-            j["data"]["ship"]["symbol"], self.session, j["data"]["ship"]
-        ), ShipyardTransaction(j["data"]["transaction"])
+        if "description" in data:
+            self.description = data["description"]
+        else:
+            self.description = None
+        if "condition" in data:
+            self.condition = data["condition"]
+        else:
+            self.condition = 100
+        self.requirements = Requirements(data["requirements"])
+
+
+class Frame(ShipComponent):
+    def __init__(self, data):
+        super().__init__(data)
+        self.module_slots = data["moduleSlots"]
+        self.mounting_points = data["mountingPoints"]
+        self.fuel_capacity = data["fuelCapacity"]
+
+
+class Reactor(ShipComponent):
+    def __init__(self, data):
+        super().__init__(data)
+        self.power_output = data["powerOutput"]
+        self.cooldown: Optional[datetime] = None
+
+
+class Engine(ShipComponent):
+    def __init__(self, data):
+        super().__init__(data)
+        self.speed = data["speed"]
+
+
+class Module(ShipComponent):
+    def __init__(self, data):
+        super().__init__(data)
+        if "capacity" in data:
+            self.capacity = data["capacity"]
+        if "range" in data:
+            self.range = data["range"]
+
+
+class Mount(ShipComponent):
+    def __init__(self, data):
+        super().__init__(data)
+        if "strength" in data:
+            self.strength = data["strength"]
+        if "deposits" in data:
+            self.deposits = data["deposits"]
```

### Comparing `autotraders-1.6.4/autotraders/paginated_list.py` & `autotraders-1.7.0/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/session.py` & `autotraders-1.7.0/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/shared_models/map_symbol.py` & `autotraders-1.7.0/autotraders/shared_models/map_symbol.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,23 +22,22 @@
             raise ValueError("Invalid map symbol")
         self.raw = s
 
     def __str__(self):
         """Returns the input that was passed as a string."""
         return self.raw
 
+    def __hash__(self):
+        return self.raw
+
     def __add__(self, other):
         return self / other
 
     def __truediv__(self, other):
         """Concatenates with a '-'"""
         assert isinstance(other, str)
         if other[0] == "-":
             other = other[1:]
         return MapSymbol(str(self) + "-" + other)
 
     def __eq__(self, other):
-        return (
-            self.sector == other.sector
-            and self.system == other.system
-            and self.waypoint == other.waypoint
-        )
+        return str(self) == str(other)
```

### Comparing `autotraders-1.6.4/autotraders/shared_models/transaction.py` & `autotraders-1.7.0/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/ship/__init__.py` & `autotraders-1.7.0/autotraders/ship/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,21 @@
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return Item(
             j["data"]["extraction"]["yield"]["symbol"],
             j["data"]["extraction"]["yield"]["units"],
             None,
         )
 
-    def refuel(self):
-        j = self.post("refuel")
+    def refuel(self, units=None):
+        if units is None:
+            j = self.post("refuel")
+        else:
+            j = self.post("refuel", data={
+                "units": units
+            })
         self.update(j["data"])
         return MarketTransaction(j["data"]["transaction"])
 
     def sell(self, cargo_symbol: str, quantity: int):
         j = self.post("sell", data={"symbol": cargo_symbol, "units": quantity})
         self.update(j["data"])
         return MarketTransaction(j["data"]["transaction"])
```

### Comparing `autotraders-1.6.4/autotraders/ship/cargo.py` & `autotraders-1.7.0/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/ship/nav.py` & `autotraders-1.7.0/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/space_traders_entity.py` & `autotraders-1.7.0/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/status.py` & `autotraders-1.7.0/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders/util.py` & `autotraders-1.7.0/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/autotraders.egg-info/PKG-INFO` & `autotraders-1.7.0/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.6.4
+Version: 1.7.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://comsictraders.github.io/autotraders/
 Project-URL: Repository, https://github.com/comsictraders/autotraders.git
 Project-URL: Changelog, https://github.com/comsictraders/autotraders/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://comsictraders.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/comsictraders/autotraders/issues
```

### Comparing `autotraders-1.6.4/autotraders.egg-info/SOURCES.txt` & `autotraders-1.7.0/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/pyproject.toml` & `autotraders-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/tests/test_init.py` & `autotraders-1.7.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/tests/test_map.py` & `autotraders-1.7.0/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.6.4/tests/test_ship.py` & `autotraders-1.7.0/tests/test_ship.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from datetime import datetime, timedelta, timezone
 
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship import Ship, Nav
+from autotraders.ship.states import NavState
 from test_init import session
 
 
 def test_ship(session):
     Ship("TEST", session)
 
 
 def test_ship_functions(session):
     s = Ship("TEST", session)
     s.update_ship_cooldown()
     s.dock()
     s.orbit()
     s.refuel()
+    s.refuel(999)
     s.extract()
 
 
 def test_ship_mount_functions(session):
     s = Ship("TEST", session)
     s.install_mount("TEST_MOUNT")
     s.remove_mount("TEST_MOUNT")
@@ -64,20 +66,21 @@
     assert n.moving
     start2 = datetime.now(timezone.utc) - timedelta(seconds=10)
     end2 = datetime.now(timezone.utc) - timedelta(seconds=5)
     n2 = Nav(
         "MOCK_SHIP_SYMBOL",
         session,
         {
-            "status": "ORBIT",
+            "status": "IN_ORBIT",
             "waypointSymbol": "X1-TEST-TEST2",
             "flightMode": "CRUISE",
             "route": {
                 "destination": {"symbol": "X1-TEST-TEST2"},
                 "departure": {"symbol": "X1-TEST-TEST"},
                 "departureTime": start2.strftime("%Y-%m-%dT%H:%M:%SZ"),
                 "arrival": end2.strftime("%Y-%m-%dT%H:%M:%SZ"),
             },
         },
     )
-    assert n2.status == "ORBIT"
+    assert n2.status == "IN_ORBIT"
+    assert n2.status == NavState.IN_ORBIT
     assert not n2.moving
```

### Comparing `autotraders-1.6.4/tests/test_util.py` & `autotraders-1.7.0/tests/test_util.py`

 * *Files identical despite different names*

