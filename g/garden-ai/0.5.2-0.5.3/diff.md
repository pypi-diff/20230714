# Comparing `tmp/garden_ai-0.5.2.tar.gz` & `tmp/garden_ai-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.5.2.tar", max compression
+gzip compressed data, was "garden_ai-0.5.3.tar", max compression
```

## Comparing `garden_ai-0.5.2.tar` & `garden_ai-0.5.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1078 2023-07-13 20:51:41.118266 garden_ai-0.5.2/LICENSE
--rw-r--r--   0        0        0      797 2023-07-13 20:51:41.118266 garden_ai-0.5.2/README.md
--rw-r--r--   0        0        0      418 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/__main__.py
--rw-r--r--   0        0        0     4454 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/_model.py
--rw-r--r--   0        0        0      180 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/__init__.py
--rw-r--r--   0        0        0     2855 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/console.py
--rw-r--r--   0        0        0    11506 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/main.py
--rw-r--r--   0        0        0     3895 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/model.py
--rw-r--r--   0        0        0    11770 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0     4002 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/backend_client.py
--rw-r--r--   0        0        0    18653 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/client.py
--rw-r--r--   0        0        0      440 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/constants.py
--rw-r--r--   0        0        0     9394 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/datacite.py
--rw-r--r--   0        0        0    14824 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2802 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1603 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      798 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7553 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/local_data.py
--rw-r--r--   0        0        0     8126 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/mlmodel.py
--rw-r--r--   0        0        0        0 2023-07-13 20:51:41.118266 garden_ai-0.5.2/garden_ai/model_file_transfer/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/model_file_transfer/upload.py
--rw-r--r--   0        0        0    19626 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/pipelines.py
--rw-r--r--   0        0        0    10745 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/steps.py
--rw-r--r--   0        0        0     2019 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     5258 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/_meta.py
--rw-r--r--   0        0        0     1018 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0     8533 2023-07-13 20:51:41.122266 garden_ai-0.5.2/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2867 2023-07-13 20:51:53.382439 garden_ai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 garden_ai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-14 16:00:50.387446 garden_ai-0.5.3/LICENSE
+-rw-r--r--   0        0        0      797 2023-07-14 16:00:50.387446 garden_ai-0.5.3/README.md
+-rw-r--r--   0        0        0      418 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/__main__.py
+-rw-r--r--   0        0        0     4454 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/_model.py
+-rw-r--r--   0        0        0      180 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/console.py
+-rw-r--r--   0        0        0    11506 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/main.py
+-rw-r--r--   0        0        0     3895 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/model.py
+-rw-r--r--   0        0        0    11770 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0     4002 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    18710 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/client.py
+-rw-r--r--   0        0        0      440 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/constants.py
+-rw-r--r--   0        0        0     9394 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/datacite.py
+-rw-r--r--   0        0        0    14824 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2802 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1603 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      798 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7553 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/local_data.py
+-rw-r--r--   0        0        0     8176 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/model_file_transfer/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/model_file_transfer/upload.py
+-rw-r--r--   0        0        0    19626 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    10745 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/steps.py
+-rw-r--r--   0        0        0     2019 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     5258 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0     1018 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0     8533 2023-07-14 16:00:50.391446 garden_ai-0.5.3/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2903 2023-07-14 16:01:03.123311 garden_ai-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 garden_ai-0.5.3/PKG-INFO
```

### Comparing `garden_ai-0.5.2/LICENSE` & `garden_ai-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/README.md` & `garden_ai-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/_model.py` & `garden_ai-0.5.3/garden_ai/_model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/app/console.py` & `garden_ai-0.5.3/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/app/garden.py` & `garden_ai-0.5.3/garden_ai/app/garden.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/app/main.py` & `garden_ai-0.5.3/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/app/model.py` & `garden_ai-0.5.3/garden_ai/app/model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/app/pipeline.py` & `garden_ai-0.5.3/garden_ai/app/pipeline.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/backend_client.py` & `garden_ai-0.5.3/garden_ai/backend_client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/client.py` & `garden_ai-0.5.3/garden_ai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,14 +425,15 @@
         return garden
 
     def publish_garden_metadata(self, garden: Garden) -> None:
         """
         Publishes a Garden's expanded_json to the backend /garden-search-route,
         making it visible on our Globus Search index.
         """
+        self._generate_presigned_urls_for_garden(garden)
         self._update_datacite(garden)
         try:
             self.backend_client.publish_garden_metadata(garden)
         except Exception as e:
             raise Exception(
                 f"Request to Garden backend to publish garden failed with error: {str(e)}"
             )
```

### Comparing `garden_ai-0.5.2/garden_ai/datacite.py` & `garden_ai-0.5.3/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/gardens.py` & `garden_ai-0.5.3/garden_ai/gardens.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/globus_compute/containers.py` & `garden_ai-0.5.3/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/globus_compute/login_manager.py` & `garden_ai-0.5.3/garden_ai/globus_compute/login_manager.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.5.3/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/globus_search/garden_search.py` & `garden_ai-0.5.3/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/local_data.py` & `garden_ai-0.5.3/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/mlmodel.py` & `garden_ai-0.5.3/garden_ai/mlmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,16 @@
 
     return model_dir
 
 
 def clear_mlflow_staging_directory():
     path = str(MODEL_STAGING_DIR)
     for item in os.listdir(path):
+        if item == ".trash":
+            continue
         item_path = os.path.join(path, item)
         if os.path.isfile(item_path):
             os.remove(item_path)
         elif os.path.isdir(item_path):
             shutil.rmtree(item_path)
```

### Comparing `garden_ai-0.5.2/garden_ai/model_file_transfer/upload.py` & `garden_ai-0.5.3/garden_ai/model_file_transfer/upload.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/pipelines.py` & `garden_ai-0.5.3/garden_ai/pipelines.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/steps.py` & `garden_ai-0.5.3/garden_ai/steps.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/templates/pipeline` & `garden_ai-0.5.3/garden_ai/templates/pipeline`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/utils/_meta.py` & `garden_ai-0.5.3/garden_ai/utils/_meta.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/utils/filesystem.py` & `garden_ai-0.5.3/garden_ai/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/garden_ai/utils/misc.py` & `garden_ai-0.5.3/garden_ai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.5.2/pyproject.toml` & `garden_ai-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "v0.5.2" # placeholder
+version = "0.5.3" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -40,15 +40,15 @@
 numba = "^0.56"
 boto3 = "^1.26.77"
 dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
 globus-compute-sdk = "^2.2.0"
 # Be sure to add additional flavors as optional below as support is added and update tool.poetry.extras
-torch = { version = "^2.0.0", optional = true }
+torch = { version = "^2.0.0, !=2.0.1", optional = true }
 tensorflow = { version = "^2.11.0", optional = true, python = ">=3.8,<3.12" }
 
 [tool.poetry.scripts]
 garden-ai = "garden_ai.app.main:app"
 
 [tool.poetry.group.test]
 optional = true
@@ -87,14 +87,15 @@
 profile = "black"
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 exclude = "/fixtures/"
 
 [tool.pytest.ini_options]
+norecursedirs = "tests/ete"
 markers = [
   "integration: deselect with '-m \"not integration\"' to run unit tests only.",
   "cli: deselect with '-m \"not cli\"' to disable CLI tests."
 ]
 
 [tool.coverage.run]
 source = ["garden_ai/"]
```

### Comparing `garden_ai-0.5.2/PKG-INFO` & `garden_ai-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.5.2
+Version: 0.5.3
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
@@ -27,15 +27,15 @@
 Requires-Dist: mlflow (>=2.4.2,<3.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "all")
-Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "all"
+Requires-Dist: torch (>=2.0.0,<3.0.0,!=2.0.1) ; extra == "torch" or extra == "all"
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://garden-ai.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Garden-AI/garden
 Description-Content-Type: text/markdown
 
 # Garden
```

