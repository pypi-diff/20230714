# Comparing `tmp/burnysc2-6.2.0.tar.gz` & `tmp/burnysc2-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burnysc2-6.2.0.tar", max compression
+gzip compressed data, was "burnysc2-6.3.0.tar", max compression
```

## Comparing `burnysc2-6.2.0.tar` & `burnysc2-6.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1072 2023-04-05 18:07:12.487543 burnysc2-6.2.0/LICENSE
--rw-r--r--   0        0        0     3501 2023-04-05 18:07:12.491543 burnysc2-6.2.0/pyproject.toml
--rw-r--r--   0        0        0      305 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/__init__.py
--rw-r--r--   0        0        0     4139 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/action.py
--rw-r--r--   0        0        0    61153 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/bot_ai.py
--rw-r--r--   0        0        0    42583 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/bot_ai_internal.py
--rw-r--r--   0        0        0     1807 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/cache.py
--rw-r--r--   0        0        0    36292 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/client.py
--rw-r--r--   0        0        0    25400 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/constants.py
--rw-r--r--   0        0        0     3088 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/controller.py
--rw-r--r--   0        0        0     3392 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/data.py
--rw-r--r--   0        0        0      306 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/__init__.py
--rw-r--r--   0        0        0    16982 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/generic_redirect_abilities.py
--rw-r--r--   0        0        0    39206 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/unit_abilities.py
--rw-r--r--   0        0        0    18259 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/unit_research_abilities.py
--rw-r--r--   0        0        0     2088 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/unit_tech_alias.py
--rw-r--r--   0        0        0    21568 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/unit_train_build_abilities.py
--rw-r--r--   0        0        0     5830 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/unit_trained_from.py
--rw-r--r--   0        0        0     2521 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/unit_unit_alias.py
--rw-r--r--   0        0        0     5668 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/dicts/upgrade_researched_from.py
--rw-r--r--   0        0        0     5640 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/expiring_dict.py
--rw-r--r--   0        0        0    12982 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/game_data.py
--rw-r--r--   0        0        0    14000 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/game_info.py
--rw-r--r--   0        0        0    12317 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/game_state.py
--rw-r--r--   0        0        0     8590 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/generate_ids.py
--rw-r--r--   0        0        0      191 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/__init__.py
--rw-r--r--   0        0        0    52948 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/ability_id.py
--rw-r--r--   0        0        0     9427 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/buff_id.py
--rw-r--r--   0        0        0      685 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/effect_id.py
--rw-r--r--   0        0        0       35 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/id_version.py
--rw-r--r--   0        0        0    63891 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/unit_typeid.py
--rw-r--r--   0        0        0     9494 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/ids/upgrade_id.py
--rw-r--r--   0        0        0    29769 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/main.py
--rw-r--r--   0        0        0     1558 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/maps.py
--rw-r--r--   0        0        0     5773 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/observer_ai.py
--rw-r--r--   0        0        0     4699 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/paths.py
--rw-r--r--   0        0        0     4181 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/pixel_map.py
--rw-r--r--   0        0        0     7021 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/player.py
--rw-r--r--   0        0        0     2854 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/portconfig.py
--rw-r--r--   0        0        0    13130 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/position.py
--rw-r--r--   0        0        0      883 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/power_source.py
--rw-r--r--   0        0        0     3014 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/protocol.py
--rw-r--r--   0        0        0    10401 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/proxy.py
--rw-r--r--   0        0        0     5817 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/renderer.py
--rw-r--r--   0        0        0     9635 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/sc2process.py
--rw-r--r--   0        0        0    11941 2023-04-05 18:07:12.495543 burnysc2-6.2.0/sc2/score.py
--rw-r--r--   0        0        0    59173 2023-04-05 18:07:12.499543 burnysc2-6.2.0/sc2/unit.py
--rw-r--r--   0        0        0     1404 2023-04-05 18:07:12.499543 burnysc2-6.2.0/sc2/unit_command.py
--rw-r--r--   0        0        0    29208 2023-04-05 18:07:12.499543 burnysc2-6.2.0/sc2/units.py
--rw-r--r--   0        0        0    17314 2023-04-05 18:07:12.499543 burnysc2-6.2.0/sc2/versions.py
--rw-r--r--   0        0        0     4155 2023-04-05 18:07:12.499543 burnysc2-6.2.0/sc2/wsl.py
--rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 burnysc2-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-14 21:38:46.401621 burnysc2-6.3.0/LICENSE
+-rw-r--r--   0        0        0     3487 2023-07-14 21:38:46.405621 burnysc2-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/__init__.py
+-rw-r--r--   0        0        0     4139 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/action.py
+-rw-r--r--   0        0        0    61153 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/bot_ai.py
+-rw-r--r--   0        0        0    43060 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/bot_ai_internal.py
+-rw-r--r--   0        0        0     1807 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/cache.py
+-rw-r--r--   0        0        0    36292 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/client.py
+-rw-r--r--   0        0        0    25400 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/constants.py
+-rw-r--r--   0        0        0     3088 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/controller.py
+-rw-r--r--   0        0        0     3392 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/data.py
+-rw-r--r--   0        0        0      306 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/__init__.py
+-rw-r--r--   0        0        0    16982 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/generic_redirect_abilities.py
+-rw-r--r--   0        0        0    39206 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_abilities.py
+-rw-r--r--   0        0        0    18259 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_research_abilities.py
+-rw-r--r--   0        0        0     2088 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_tech_alias.py
+-rw-r--r--   0        0        0    21568 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_train_build_abilities.py
+-rw-r--r--   0        0        0     5830 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_trained_from.py
+-rw-r--r--   0        0        0     2521 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/unit_unit_alias.py
+-rw-r--r--   0        0        0     5668 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/dicts/upgrade_researched_from.py
+-rw-r--r--   0        0        0     5640 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/expiring_dict.py
+-rw-r--r--   0        0        0    12982 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/game_data.py
+-rw-r--r--   0        0        0    14000 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/game_info.py
+-rw-r--r--   0        0        0    12317 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/game_state.py
+-rw-r--r--   0        0        0     8590 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/generate_ids.py
+-rw-r--r--   0        0        0      191 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/__init__.py
+-rw-r--r--   0        0        0    52948 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/ability_id.py
+-rw-r--r--   0        0        0     9427 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/buff_id.py
+-rw-r--r--   0        0        0      685 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/effect_id.py
+-rw-r--r--   0        0        0       35 2023-07-14 21:38:46.405621 burnysc2-6.3.0/sc2/ids/id_version.py
+-rw-r--r--   0        0        0    63891 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/ids/unit_typeid.py
+-rw-r--r--   0        0        0     9494 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/ids/upgrade_id.py
+-rw-r--r--   0        0        0    29769 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/main.py
+-rw-r--r--   0        0        0     1558 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/maps.py
+-rw-r--r--   0        0        0     5773 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/observer_ai.py
+-rw-r--r--   0        0        0     4699 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/paths.py
+-rw-r--r--   0        0        0     4181 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/pixel_map.py
+-rw-r--r--   0        0        0     7021 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/player.py
+-rw-r--r--   0        0        0     2854 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/portconfig.py
+-rw-r--r--   0        0        0    13130 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/position.py
+-rw-r--r--   0        0        0      883 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/power_source.py
+-rw-r--r--   0        0        0     3014 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/protocol.py
+-rw-r--r--   0        0        0    10401 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/proxy.py
+-rw-r--r--   0        0        0     5817 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/renderer.py
+-rw-r--r--   0        0        0     9635 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/sc2process.py
+-rw-r--r--   0        0        0    11941 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/score.py
+-rw-r--r--   0        0        0    59173 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/unit.py
+-rw-r--r--   0        0        0     1404 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/unit_command.py
+-rw-r--r--   0        0        0    29208 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/units.py
+-rw-r--r--   0        0        0    17314 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/versions.py
+-rw-r--r--   0        0        0     4155 2023-07-14 21:38:46.409621 burnysc2-6.3.0/sc2/wsl.py
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 burnysc2-6.3.0/PKG-INFO
```

### Comparing `burnysc2-6.2.0/LICENSE` & `burnysc2-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/pyproject.toml` & `burnysc2-6.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burnysc2"
-version = "6.2.0"
+version = "6.3.0"
 description = "A StarCraft II API Client for Python 3"
 authors = ["BurnySc2 <gamingburny@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Burnysc2/python-sc2"
 documentation = "https://burnysc2.github.io/python-sc2/docs/index.html"
 keywords = ["StarCraft", "StarCraft 2", "StarCraft II", "AI", "Bot"]
 classifiers=[
@@ -36,17 +36,16 @@
 mpyq = "^0.2.5"
 numpy = "^1.19.3"
 portpicker = "^1.4.0"
 s2clientprotocol = "^5.0.7"
 scipy = "^1.7.1"
 protobuf = "<4.0.0"
 
-[tool.poetry.dev-dependencies]
-codecov = "^2.1.12"
-coverage = "^7.0"
+[tool.poetry.group.dev.dependencies]
+coverage = "^7.2"
 hypothesis = "^6.23.1"
 matplotlib = "^3.4.3"
 mypy = "^0.960"
 pillow = "^9.0"
 pre-commit = "^2.15.0"
 pyglet = "^2.0"
 pylint = "^2.11.1"
```

### Comparing `burnysc2-6.2.0/sc2/action.py` & `burnysc2-6.3.0/sc2/action.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/bot_ai.py` & `burnysc2-6.3.0/sc2/bot_ai.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/bot_ai_internal.py` & `burnysc2-6.3.0/sc2/bot_ai_internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,21 +181,27 @@
         # Create a group for every resource
         resource_groups: List[List[Unit]] = [
             [resource] for resource in self.resources
             if resource.name != "MineralField450"  # dont use low mineral count patches
         ]
         # Loop the merging process as long as we change something
         merged_group = True
+        height_grid: PixelMap = self.game_info.terrain_height
         while merged_group:
             merged_group = False
             # Check every combination of two groups
             for group_a, group_b in itertools.combinations(resource_groups, 2):
                 # Check if any pair of resource of these groups is closer than threshold together
+                # And that they are on the same terrain level
                 if any(
                     resource_a.distance_to(resource_b) <= resource_spread_threshold
+                    # check if terrain height measurement at resources is within 10 units
+                    # this is since some older maps have inconsistent terrain height
+                    # tiles at certain expansion locations
+                    and abs(height_grid[resource_a.position.rounded] - height_grid[resource_b.position.rounded]) <= 10
                     for resource_a, resource_b in itertools.product(group_a, group_b)
                 ):
                     # Remove the single groups and add the merged group
                     resource_groups.remove(group_a)
                     resource_groups.remove(group_b)
                     resource_groups.append(group_a + group_b)
                     merged_group = True
```

### Comparing `burnysc2-6.2.0/sc2/cache.py` & `burnysc2-6.3.0/sc2/cache.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/client.py` & `burnysc2-6.3.0/sc2/client.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/constants.py` & `burnysc2-6.3.0/sc2/constants.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/controller.py` & `burnysc2-6.3.0/sc2/controller.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/data.py` & `burnysc2-6.3.0/sc2/data.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/generic_redirect_abilities.py` & `burnysc2-6.3.0/sc2/dicts/generic_redirect_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/unit_abilities.py` & `burnysc2-6.3.0/sc2/dicts/unit_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/unit_research_abilities.py` & `burnysc2-6.3.0/sc2/dicts/unit_research_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/unit_tech_alias.py` & `burnysc2-6.3.0/sc2/dicts/unit_tech_alias.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/unit_train_build_abilities.py` & `burnysc2-6.3.0/sc2/dicts/unit_train_build_abilities.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/unit_trained_from.py` & `burnysc2-6.3.0/sc2/dicts/unit_trained_from.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/unit_unit_alias.py` & `burnysc2-6.3.0/sc2/dicts/unit_unit_alias.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/dicts/upgrade_researched_from.py` & `burnysc2-6.3.0/sc2/dicts/upgrade_researched_from.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/expiring_dict.py` & `burnysc2-6.3.0/sc2/expiring_dict.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/game_data.py` & `burnysc2-6.3.0/sc2/game_data.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/game_info.py` & `burnysc2-6.3.0/sc2/game_info.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/game_state.py` & `burnysc2-6.3.0/sc2/game_state.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/generate_ids.py` & `burnysc2-6.3.0/sc2/generate_ids.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/ids/ability_id.py` & `burnysc2-6.3.0/sc2/ids/ability_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/ids/buff_id.py` & `burnysc2-6.3.0/sc2/ids/buff_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/ids/effect_id.py` & `burnysc2-6.3.0/sc2/ids/effect_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/ids/unit_typeid.py` & `burnysc2-6.3.0/sc2/ids/unit_typeid.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/ids/upgrade_id.py` & `burnysc2-6.3.0/sc2/ids/upgrade_id.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/main.py` & `burnysc2-6.3.0/sc2/main.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/maps.py` & `burnysc2-6.3.0/sc2/maps.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/observer_ai.py` & `burnysc2-6.3.0/sc2/observer_ai.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/paths.py` & `burnysc2-6.3.0/sc2/paths.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/pixel_map.py` & `burnysc2-6.3.0/sc2/pixel_map.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/player.py` & `burnysc2-6.3.0/sc2/player.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/portconfig.py` & `burnysc2-6.3.0/sc2/portconfig.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/position.py` & `burnysc2-6.3.0/sc2/position.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/power_source.py` & `burnysc2-6.3.0/sc2/power_source.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/protocol.py` & `burnysc2-6.3.0/sc2/protocol.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/proxy.py` & `burnysc2-6.3.0/sc2/proxy.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/renderer.py` & `burnysc2-6.3.0/sc2/renderer.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/sc2process.py` & `burnysc2-6.3.0/sc2/sc2process.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/score.py` & `burnysc2-6.3.0/sc2/score.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/unit.py` & `burnysc2-6.3.0/sc2/unit.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/unit_command.py` & `burnysc2-6.3.0/sc2/unit_command.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/units.py` & `burnysc2-6.3.0/sc2/units.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/versions.py` & `burnysc2-6.3.0/sc2/versions.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/sc2/wsl.py` & `burnysc2-6.3.0/sc2/wsl.py`

 * *Files identical despite different names*

### Comparing `burnysc2-6.2.0/PKG-INFO` & `burnysc2-6.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burnysc2
-Version: 6.2.0
+Version: 6.3.0
 Summary: A StarCraft II API Client for Python 3
 Home-page: https://github.com/Burnysc2/python-sc2
 License: MIT
 Keywords: StarCraft,StarCraft 2,StarCraft II,AI,Bot
 Author: BurnySc2
 Author-email: gamingburny@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -16,19 +16,14 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mpyq (>=0.2.5,<0.3.0)
```

