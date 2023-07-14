# Comparing `tmp/f1_telemetry-2023.1.1.tar.gz` & `tmp/f1_telemetry-2023.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f1_telemetry-2023.1.1.tar", max compression
+gzip compressed data, was "f1_telemetry-2023.1.2.tar", max compression
```

## Comparing `f1_telemetry-2023.1.1.tar` & `f1_telemetry-2023.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1791 2023-07-13 16:57:07.260811 f1_telemetry-2023.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/__init__.py
--rw-r--r--   0        0        0     2307 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/__main__.py
--rw-r--r--   0        0        0    16287 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/collector.py
--rw-r--r--   0        0        0     1155 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/live.py
--rw-r--r--   0        0        0     6082 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/model.py
--rw-r--r--   0        0        0     2878 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/report.py
--rw-r--r--   0        0        0      467 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/server.py
--rw-r--r--   0        0        0     1393 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/storage.py
--rw-r--r--   0        0        0     2742 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/view.py
--rw-r--r--   0        0        0    73384 2023-07-13 16:57:07.280812 f1_telemetry-2023.1.1/f1_telemetry/webapp/art/Formula1-Regular.ttf
--rw-r--r--   0        0        0   203029 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/art/bg.jpg
--rw-r--r--   0        0        0    33104 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/art/car.svg
--rw-r--r--   0        0        0     5266 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/index.html
--rw-r--r--   0        0        0    35177 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/live.html
--rw-r--r--   0        0        0     6497 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/live.js
--rw-r--r--   0        0        0     9991 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/plots.js
--rw-r--r--   0        0        0     4647 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/queries.js
--rw-r--r--   0        0        0     1321 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/style.css
--rw-r--r--   0        0        0     3189 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/trace.js
--rw-r--r--   0        0        0      787 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/utils.js
--rw-r--r--   0        0        0     6089 2023-07-13 16:57:07.284812 f1_telemetry-2023.1.1/f1_telemetry/webapp/view.js
--rw-r--r--   0        0        0     1078 2023-07-13 16:57:22.944928 f1_telemetry-2023.1.1/pyproject.toml
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 f1_telemetry-2023.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1791 2023-07-14 17:44:45.006978 f1_telemetry-2023.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/__init__.py
+-rw-r--r--   0        0        0     2307 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/__main__.py
+-rw-r--r--   0        0        0    16287 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/collector.py
+-rw-r--r--   0        0        0     1155 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/live.py
+-rw-r--r--   0        0        0     6097 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/model.py
+-rw-r--r--   0        0        0     2883 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/report.py
+-rw-r--r--   0        0        0      467 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/server.py
+-rw-r--r--   0        0        0     1393 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/storage.py
+-rw-r--r--   0        0        0     2742 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/view.py
+-rw-r--r--   0        0        0    73384 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/webapp/art/Formula1-Regular.ttf
+-rw-r--r--   0        0        0   203029 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/art/bg.jpg
+-rw-r--r--   0        0        0    33104 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/art/car.svg
+-rw-r--r--   0        0        0     5266 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/index.html
+-rw-r--r--   0        0        0    35177 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/live.html
+-rw-r--r--   0        0        0     6497 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/live.js
+-rw-r--r--   0        0        0     9991 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/plots.js
+-rw-r--r--   0        0        0     4647 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/queries.js
+-rw-r--r--   0        0        0     1321 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/style.css
+-rw-r--r--   0        0        0     3189 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/trace.js
+-rw-r--r--   0        0        0      787 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/utils.js
+-rw-r--r--   0        0        0     6089 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/view.js
+-rw-r--r--   0        0        0     1078 2023-07-14 17:44:56.462948 f1_telemetry-2023.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 f1_telemetry-2023.1.2/PKG-INFO
```

### Comparing `f1_telemetry-2023.1.1/README.md` & `f1_telemetry-2023.1.2/README.md`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/__main__.py` & `f1_telemetry-2023.1.2/f1_telemetry/__main__.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/collector.py` & `f1_telemetry-2023.1.2/f1_telemetry/collector.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/live.py` & `f1_telemetry-2023.1.2/f1_telemetry/live.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/model.py` & `f1_telemetry-2023.1.2/f1_telemetry/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,17 +191,17 @@
 
     def lap_data(self, data: LapData):
         self._lap_data = data
 
         self.step()
 
     def car_status_data(self, data: CarStatusData):
-        self.tyre = {16: "Soft", 17: "Medium", 18: "Hard", 7: "Inter", 8: "Wet"}[
-            data.visual_tyre_compound
-        ]
+        self.tyre = {16: "Soft", 17: "Medium", 18: "Hard", 7: "Inter", 8: "Wet"}.get(
+            data.visual_tyre_compound, "Unknown"
+        )
         self.tyre_age = data.tyres_age_laps
 
     def final_classification(self):
         self.state = SessionState.FINISHED
 
         self.step()
```

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/report.py` & `f1_telemetry-2023.1.2/f1_telemetry/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 class RaceReport(Report):
     def rows(self):
         final_data = []
         for i, name in self.drivers.items():
             data = self.data[i]
 
-            total_time = (data.total_race_time + data.penalties_time) * 1000
+            total_time = int((data.total_race_time + data.penalties_time) * 1000)
 
             final_data.append(
                 (
                     data.position,
                     name,
                     data.best_lap_time_in_ms,
                     fmtt(data.best_lap_time_in_ms),
```

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/storage.py` & `f1_telemetry-2023.1.2/f1_telemetry/storage.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/view.py` & `f1_telemetry-2023.1.2/f1_telemetry/view.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/art/Formula1-Regular.ttf` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/art/Formula1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/art/bg.jpg` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/art/bg.jpg`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/art/car.svg` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/art/car.svg`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/index.html` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/index.html`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/live.html` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/live.html`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/live.js` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/live.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/plots.js` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/plots.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/queries.js` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/queries.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/style.css` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/style.css`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/trace.js` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/trace.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/utils.js` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/utils.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/f1_telemetry/webapp/view.js` & `f1_telemetry-2023.1.2/f1_telemetry/webapp/view.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.1/pyproject.toml` & `f1_telemetry-2023.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 authors = ["Gabriele N. Tornetta <phoenix1987@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "f1_telemetry"},
 ]
 readme = "README.md"
 repository = "https://github.com/P403n1x87/f1-telemetry"
-version = "2023.1.1"
+version = "2023.1.2"
 
 [tool.isort]
 force_single_line = true
 lines_after_imports = 2
 profile = "black"
 
 [tool.poetry.dependencies]
```

### Comparing `f1_telemetry-2023.1.1/PKG-INFO` & `f1_telemetry-2023.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f1-telemetry
-Version: 2023.1.1
+Version: 2023.1.2
 Summary: F1 telemetry data collection and visualisation
 Home-page: https://github.com/P403n1x87/f1-telemetry
 License: MIT
 Author: Gabriele N. Tornetta
 Author-email: phoenix1987@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

