# Comparing `tmp/reverse-projection-0.0.2.4.tar.gz` & `tmp/reverse-projection-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse-projection-0.0.2.4.tar", last modified: Mon Dec 12 01:31:28 2022, max compression
+gzip compressed data, was "reverse-projection-0.0.2.5.tar", last modified: Fri Jul 14 04:44:44 2023, max compression
```

## Comparing `reverse-projection-0.0.2.4.tar` & `reverse-projection-0.0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 01:31:28.044755 reverse-projection-0.0.2.4/
--rw-rw-rw-   0        0        0      436 2022-12-12 01:31:28.043757 reverse-projection-0.0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-12 01:31:28.024806 reverse-projection-0.0.2.4/reverse_projection/
--rw-rw-rw-   0        0        0       37 2022-10-30 13:51:17.000000 reverse-projection-0.0.2.4/reverse_projection/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-12 01:31:28.032785 reverse-projection-0.0.2.4/reverse_projection/search/
--rw-rw-rw-   0        0        0       35 2022-04-27 12:27:06.000000 reverse-projection-0.0.2.4/reverse_projection/search/__init__.py
--rw-rw-rw-   0        0        0     3488 2022-10-07 07:54:57.000000 reverse-projection-0.0.2.4/reverse_projection/search/algorithms.py
--rw-rw-rw-   0        0        0     8713 2022-10-07 07:02:16.000000 reverse-projection-0.0.2.4/reverse_projection/search/main.py
-drwxrwxrwx   0        0        0        0 2022-12-12 01:31:28.039766 reverse-projection-0.0.2.4/reverse_projection/webapis/
--rw-rw-rw-   0        0        0        0 2022-09-16 13:50:12.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/__init__.py
--rw-rw-rw-   0        0        0    17032 2022-11-29 07:07:35.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/algorithms.py
--rw-rw-rw-   0        0        0     1431 2022-10-03 09:33:19.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/configs.py
--rw-rw-rw-   0        0        0     5094 2022-10-12 06:00:13.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/data.py
--rw-rw-rw-   0        0        0    25308 2022-12-09 03:03:14.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/db.py
--rw-rw-rw-   0        0        0     3690 2022-09-23 08:52:34.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/decomposers.py
--rw-rw-rw-   0        0        0     8614 2022-09-26 12:15:45.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/targets.py
--rw-rw-rw-   0        0        0      905 2022-11-11 07:10:32.000000 reverse-projection-0.0.2.4/reverse_projection/webapis/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-12 01:31:28.030790 reverse-projection-0.0.2.4/reverse_projection.egg-info/
--rw-rw-rw-   0        0        0      436 2022-12-12 01:31:27.000000 reverse-projection-0.0.2.4/reverse_projection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2022-12-12 01:31:27.000000 reverse-projection-0.0.2.4/reverse_projection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 01:31:27.000000 reverse-projection-0.0.2.4/reverse_projection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-12-12 01:31:27.000000 reverse-projection-0.0.2.4/reverse_projection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-12-12 01:31:27.000000 reverse-projection-0.0.2.4/reverse_projection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-12 01:31:28.044755 reverse-projection-0.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      971 2022-12-12 01:31:13.000000 reverse-projection-0.0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-12 01:31:28.042760 reverse-projection-0.0.2.4/test/
--rw-rw-rw-   0        0        0     3117 2022-09-17 06:40:01.000000 reverse-projection-0.0.2.4/test/test_Targets.py
--rw-rw-rw-   0        0        0     1003 2022-09-25 04:10:41.000000 reverse-projection-0.0.2.4/test/test_decision_functions.py
--rw-rw-rw-   0        0        0      998 2022-09-17 15:52:02.000000 reverse-projection-0.0.2.4/test/test_decomposition.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:44:44.513025 reverse-projection-0.0.2.5/
+-rw-rw-rw-   0        0        0      436 2023-07-14 04:44:44.512026 reverse-projection-0.0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 04:44:44.481108 reverse-projection-0.0.2.5/reverse_projection/
+-rw-rw-rw-   0        0        0       37 2022-10-30 13:51:17.000000 reverse-projection-0.0.2.5/reverse_projection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:44:44.495070 reverse-projection-0.0.2.5/reverse_projection/search/
+-rw-rw-rw-   0        0        0       35 2022-04-27 12:27:06.000000 reverse-projection-0.0.2.5/reverse_projection/search/__init__.py
+-rw-rw-rw-   0        0        0     3488 2022-10-07 07:54:57.000000 reverse-projection-0.0.2.5/reverse_projection/search/algorithms.py
+-rw-rw-rw-   0        0        0     8713 2022-10-07 07:02:16.000000 reverse-projection-0.0.2.5/reverse_projection/search/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:44:44.507037 reverse-projection-0.0.2.5/reverse_projection/webapis/
+-rw-rw-rw-   0        0        0        0 2022-09-16 13:50:12.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/__init__.py
+-rw-rw-rw-   0        0        0    18993 2023-01-22 10:44:26.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/algorithms.py
+-rw-rw-rw-   0        0        0     1431 2022-10-03 09:33:19.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/configs.py
+-rw-rw-rw-   0        0        0     5094 2022-10-12 06:00:13.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/data.py
+-rw-rw-rw-   0        0        0    25697 2023-07-14 04:28:04.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/db.py
+-rw-rw-rw-   0        0        0     3690 2022-09-23 08:52:34.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/decomposers.py
+-rw-rw-rw-   0        0        0     8614 2022-09-26 12:15:45.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/targets.py
+-rw-rw-rw-   0        0        0      905 2023-07-14 04:08:21.000000 reverse-projection-0.0.2.5/reverse_projection/webapis/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:44:44.491081 reverse-projection-0.0.2.5/reverse_projection.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-07-14 04:44:43.000000 reverse-projection-0.0.2.5/reverse_projection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-07-14 04:44:44.000000 reverse-projection-0.0.2.5/reverse_projection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:44:43.000000 reverse-projection-0.0.2.5/reverse_projection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-07-14 04:44:44.000000 reverse-projection-0.0.2.5/reverse_projection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-14 04:44:44.000000 reverse-projection-0.0.2.5/reverse_projection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:44:44.513025 reverse-projection-0.0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-14 04:43:58.000000 reverse-projection-0.0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:44:44.511030 reverse-projection-0.0.2.5/test/
+-rw-rw-rw-   0        0        0     3117 2022-09-17 06:40:01.000000 reverse-projection-0.0.2.5/test/test_Targets.py
+-rw-rw-rw-   0        0        0     1003 2022-09-25 04:10:41.000000 reverse-projection-0.0.2.5/test/test_decision_functions.py
+-rw-rw-rw-   0        0        0      998 2022-09-17 15:52:02.000000 reverse-projection-0.0.2.5/test/test_decomposition.py
```

### Comparing `reverse-projection-0.0.2.4/reverse_projection/search/algorithms.py` & `reverse-projection-0.0.2.5/reverse_projection/search/algorithms.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection/search/main.py` & `reverse-projection-0.0.2.5/reverse_projection/search/main.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/algorithms.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/algorithms.py`

 * *Files 10% similar despite different names*

```diff
@@ -301,14 +301,19 @@
 
     @property
     def decision_function(self) -> dict:
         if self.decomposer in ["pca"] and self.scaler in ["std"]:
             components = self._decomposer.components_.T
             components_ = (components.T / self._scaler.scale_).T
             original_rect_range = self.rect_range.copy()
+            if components_.shape[0] != components_.shape[1]:
+                return {
+                    "components": [],
+                    "original_rect_range": []
+                }
             tmp = np.dot(self._scaler.mean_, components_) + \
                 np.dot(self._decomposer.mean_, components.T)
             tmp = tmp[self.axis]
             for i in range(tmp.shape[0]):
                 original_rect_range[i*2: i*2+2] += tmp[i]
             return {
                 "components": components_[:, self.axis].round(3).tolist(),
@@ -347,82 +352,117 @@
             axises=self.axis,
             iteration=200,
         )
         reverse = ReverseProjection(**reverse_p)
 
         samples = self.decomposed_features[:, self.axis]
         original_samples = self.features
-        good_rect_mask, bad_rect_mask = self.rect_mask
+        good_rect_mask, bad_rect_mask, rect_mask = self.rect_mask
         good_rect_samples = samples[self.targets.gsm][good_rect_mask]
         good_original_samples = original_samples[self.targets.gsm][good_rect_mask]
         if good_original_samples.shape[0] > 0:
             original_minimum = good_original_samples.min(axis=0).round(3).tolist()
             original_maximum = good_original_samples.max(axis=0).round(3).tolist()
         else:
-            original_minimum = original_maximum = None
+            original_minimum = original_maximum = np.zeros_like(original_samples.min(axis=0)).tolist()
 
-        grsmin = []
-        grsmax = []
-        if len(good_rect_samples) > 0:
-            grsmin = good_rect_samples_mins = good_rect_samples.min(axis=0).tolist()
-            grsmax = good_rect_samples_maxs = good_rect_samples.max(axis=0).tolist()
-
-        if len(good_rect_samples) > 0:
-            zip_ = zip(grsmin, grsmax)
+        rect_samples = original_samples[rect_mask]
+        if rect_samples.shape[0] > 0:
+            rect_minimum = rect_samples.min(axis=0).round(3).tolist()
+            rect_maximum = rect_samples.max(axis=0).round(3).tolist()
         else:
-            zip_ = zip(self.rect_range[:2], self.rect_range[2:])
+            rect_minimum = rect_maximum = np.zeros_like(original_samples.min(axis=0)).tolist()
+
+        # grsmin = []
+        # grsmax = []
+        # if len(good_rect_samples) > 0:
+        #     grsmin = good_rect_samples_mins = good_rect_samples.min(axis=0).tolist()
+        #     grsmax = good_rect_samples_maxs = good_rect_samples.max(axis=0).tolist()
+
+        # if len(good_rect_samples) > 0:
+        #     zip_ = zip(grsmin, grsmax)
+        # else:
+        #     zip_ = zip(self.rect_range[:2], self.rect_range[2:])
 
         # results = []
         # for i, j in zip_:
         #     search_r = reverse.search([i, j])
         #     features = search_r["features"]
         #     features = np.reshape(features, (1, -1))
         #     features = self._scaler.inverse_transform(features)
         #     results.append(
         #         features.reshape(1, -1)
         #     )
         # results = np.concatenate([results], axis=0).round(3)
         # maximum = np.max(results, axis=0).reshape(-1, ).tolist()
         # minimum = np.min(results, axis=0).reshape(-1, ).tolist()
+        # rect_center_point = [self.rect_range[0:2].mean(), self.rect_range[2:].mean()]
+        # results = []
+        # for i in range(10):
+        #     search_r = reverse.search(rect_center_point)
+        #     features = search_r["features"]
+        #     features = np.reshape(features, (1, -1))
+        #     features = self._scaler.inverse_transform(features)
+        #     results.append(
+        #         features.reshape(1, -1)
+        #     )
+        # results = np.concatenate([results], axis=0).round(3)
+        # opt_maximum = np.max(results, axis=0).reshape(-1, ).tolist()
+        # opt_minimum = np.min(results, axis=0).reshape(-1, ).tolist()
         return {
             # "opt": [ minimum, maximum ],
             "good_mean": [
                 original_minimum, 
-                original_maximum
-            ]
+                original_maximum,
+            ],
+            "rect_mean": [
+                rect_minimum,
+                rect_maximum,
+            ],
+            # "opt_mean": [
+            #     opt_minimum,
+            #     opt_maximum,
+            # ]
         }
     
     @property
     def rect_mask(self) -> list:
         samples = self.decomposed_features[:, self.axis]
         good_samples = samples[self.targets.gsm]
         bad_samples = samples[self.targets.bsm]
 
         good_rect_mask = np.ones_like(good_samples[:, 0]).astype(bool)
         bad_rect_mask = np.ones_like(bad_samples[:, 0]).astype(bool)
+        rect_mask = np.ones_like(samples[:, 0]).astype(bool)
 
         for i in range(2):
             good_rect_mask = np.logical_and(
                 good_rect_mask, good_samples[:, i]>=self.rect_range[2*i]
             )
             good_rect_mask = np.logical_and(
                 good_rect_mask, good_samples[:, i]<=self.rect_range[2*i+1]
             )
             bad_rect_mask = np.logical_and(
                 bad_rect_mask, bad_samples[:, i]>=self.rect_range[2*i]
             )
             bad_rect_mask = np.logical_and(
                 bad_rect_mask, bad_samples[:, i]<=self.rect_range[2*i+1]
             )
-        return good_rect_mask, bad_rect_mask
+            rect_mask = np.logical_and(
+                rect_mask, samples[:, i]>=self.rect_range[2*i]
+            )
+            rect_mask = np.logical_and(
+                rect_mask, samples[:, i]<=self.rect_range[2*i+1]
+            )
+        return good_rect_mask, bad_rect_mask, rect_mask
 
     @property
     def stat_rect(self) -> list:
 
-        good_rect_mask, bad_rect_mask = self.rect_mask
+        good_rect_mask, bad_rect_mask, rect_mask = self.rect_mask
 
         good_sample_sum = good_rect_mask.astype(int).sum()
         bad_sample_sum = bad_rect_mask.astype(int).sum()
         sample_sum = good_sample_sum + bad_sample_sum
 
         results = [
             f"{sample_sum}个投影点, "
@@ -433,11 +473,14 @@
         for i, t in enumerate(self.targets):
             results.append(
                 f"目标{i}的优类均值: {round(t.regvs[self.targets.gsm][good_rect_mask].mean(), 2)}"
             )
             results.append(
                 f"目标{i}的劣类均值: {round(t.regvs[self.targets.bsm][bad_rect_mask].mean(), 2)}"
             )
+            results.append(
+                f"目标{i}的选区均值: {round(t.regvs[rect_mask].mean(), 2)}"
+            )
         return results
```

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/configs.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/configs.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/data.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/data.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/db.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 from flask import session, current_app
 import joblib
 from uuid import uuid4
 
 # from .utils import get_feature_ind
 from .data import round_data
+from .utils import get_json, get_form
 # from .algorithms import Decomposition
 
 class DBMSG:
 
     def __init__(self, state=True, message="", return_values=None) -> None:
         self.state_ = state
         self.message_ = message
@@ -57,20 +58,21 @@
     "UID": json.loads,
 
     "OTHERS": json.loads,
 }
 
 class SQLiteDB:
 
-    def __init__(self, url, init=False) -> None:
+    def __init__(self, url, user_id=None, init=False) -> None:
         self.path = Path(url)
         self.pkls = self.path.parent.joinpath("pkls")
         if not self.pkls.exists():
             self.pkls.mkdir()
         self.init = init
+        self.user_id = user_id
     
     def init_db(self) -> None:
         con = sqlite3.connect(str(self.path))
         cur = con.cursor()
         # 创建一张新的用户表
         # LEVEL -1->root, 0->default, 1->normal
         exec_str = '''
@@ -153,20 +155,28 @@
     
     def __enter__(self):
         if self.path.exists() and self.init:
             self.path.unlink()
         if not self.path.exists():
             self.init_db()
         self.con = sqlite3.connect(str(self.path))
-        try:
-            self.user_id = session.get("user_id")
-        except RuntimeError:
-            self.user_id = None
-        if not self.user_id:
-            self.user_id = 0
+        if self.user_id is None:
+            try:
+                self.user_id = session.get("user_id")
+            except RuntimeError:
+                self.user_id = None
+            if not self.user_id:
+                try:
+                    self.user_id = get_json("userId")
+                except:
+                    self.user_id = get_form("userId")
+            try:
+                self.user_id = int(self.user_id)
+            except:
+                self.user_id = 0
         return self
     
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.con.close()
         self.user_id = ""
```

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/decomposers.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/decomposers.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/targets.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/targets.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection/webapis/utils.py` & `reverse-projection-0.0.2.5/reverse_projection/webapis/utils.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/reverse_projection.egg-info/SOURCES.txt` & `reverse-projection-0.0.2.5/reverse_projection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/setup.py` & `reverse-projection-0.0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='reverse-projection',
-    version='0.0.2.4',
+    version='0.0.2.5',
     description=(
         'reverse-projection'
     ),
     author='luktian',
     author_email='luktian05@gmail.com',
     maintainer='luktian',
     maintainer_email='luktian@gmail.com',
@@ -23,15 +23,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     install_requires=[
         'hyperopt',
         'numpy',
-        'sklearn',
+        'scikit-learn',
         'pandas',
         'scipy',
         'flask',
         'flask_cors',
         'cachelib',
         'openpyxl',
         "xlrd",
```

### Comparing `reverse-projection-0.0.2.4/test/test_Targets.py` & `reverse-projection-0.0.2.5/test/test_Targets.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/test/test_decision_functions.py` & `reverse-projection-0.0.2.5/test/test_decision_functions.py`

 * *Files identical despite different names*

### Comparing `reverse-projection-0.0.2.4/test/test_decomposition.py` & `reverse-projection-0.0.2.5/test/test_decomposition.py`

 * *Files identical despite different names*

