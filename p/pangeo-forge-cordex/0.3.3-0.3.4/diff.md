# Comparing `tmp/pangeo-forge-cordex-0.3.3.tar.gz` & `tmp/pangeo-forge-cordex-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.3.3.tar", last modified: Thu Jul 13 20:14:31 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.3.4.tar", last modified: Fri Jul 14 11:45:04 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.3.3.tar` & `pangeo-forge-cordex-0.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.575570 pangeo-forge-cordex-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.579570 pangeo-forge-cordex-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.579570 pangeo-forge-cordex-0.3.3/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.579570 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 20:14:31.000000 pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:31.583570 pangeo-forge-cordex-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-13 20:14:16.000000 pangeo-forge-cordex-0.3.3/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.484180 pangeo-forge-cordex-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.480180 pangeo-forge-cordex-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.480180 pangeo-forge-cordex-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 11:45:04.484180 pangeo-forge-cordex-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.480180 pangeo-forge-cordex-0.3.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.484180 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.484180 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 11:45:04.000000 pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-14 11:45:04.484180 pangeo-forge-cordex-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:45:04.484180 pangeo-forge-cordex-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-14 11:44:54.000000 pangeo-forge-cordex-0.3.4/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.3.3/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.3.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.3.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/.gitignore` & `pangeo-forge-cordex-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/LICENSE` & `pangeo-forge-cordex-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/PKG-INFO` & `pangeo-forge-cordex-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.3
+Version: 0.3.4
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/catalog.py` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/catalog.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/esgf_access.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 import ssl
 
 import requests
 
 from .utils import combine_response, parse_dataset_response, sort_files_by_dataset_id
 
-host = "https://esgf-data.dkrz.de/esg-search/search"
+default_host = "esgf-data.dkrz.de"
+default_url = f"https://{default_host}/esg-search/search"
 
 
 def logon(host=None):
     from pyesgf.logon import LogonManager
 
     if host is None:
-        host = "esgf-data.dkrz.de"
+        host = default_host
     lm = LogonManager(verify=True)
     if not lm.is_logged_on():
         # if we find those in environment, use them.
         if "ESGF_USER" in os.environ and "ESGF_PASSWORD" in os.environ:
             lm.logon(
                 hostname=host,
                 username=os.environ["ESGF_USER"],
@@ -37,38 +38,38 @@
     sslcontext = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH)
     sslcontext.load_verify_locations(capath=lm.esgf_certs_dir)
     sslcontext.load_cert_chain(lm.esgf_credentials)
     return sslcontext
 
 
 def request(
-    url=None,
+    url,
     project="CORDEX",
     type="File",
     **search,
 ):
-    if url is None:
-        url = host
     version = search.get("version", None)
     if type == "File" and version:
         # this does not work for File searches since version denotes here rcm_version
         del search["version"]
     elif version and version.startswith("v"):
         search["version"] = version[1:]
     params = dict(project=project, type=type, format="application/solr+json", limit=500)
     params.update(search)
     return requests.get(url, params)
 
 
 def esgf_search(
-    url="https://esgf-node.llnl.gov/esg-search/search",
+    url=None,
     files_type="OPENDAP",
     project="CORDEX",
     **search,
 ):
+    if url is None:
+        url = default_url
     response = request(url, project, "Dataset", **search)
     # return response.json()["response"]
     dset_info = parse_dataset_response(response)
     response = request(url, project, "File", **search)
     # return response.json()["response"]
     files_by_id = sort_files_by_dataset_id(response)
     responses = combine_response(dset_info, files_by_id)
```

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/recipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 def create_recipe_inputs(responses, ssl=None):
     pattern_kwargs = {}
     if ssl:
         pattern_kwargs["fsspec_open_kwargs"] = {"ssl": ssl}
     inputs = {}
     for k, v in responses.items():
+        print(f"creating recipe inputs for {k}")
         inputs[k] = {}
         urls = v["urls"]["netcdf"]
         recipe_kwargs = {}
 
         recipe_kwargs["target_chunks"] = target_chunks(v, urls[0], ssl)
         inputs[k]["urls"] = urls
         inputs[k]["recipe_kwargs"] = recipe_kwargs
@@ -64,14 +65,15 @@
 
 
 def recipe_inputs_from_iids(iids, ssl=None):
     if not isinstance(iids, list):
         iids = [iids]
     dset_responses = {}
     for iid in iids:
+        print(iid)
         facets = facets_from_iid(iid)
         dset_responses.update(esgf_search(**facets))
 
     return create_recipe_inputs(dset_responses, ssl)
 
 
 def create_recipe(urls, recipe_kwargs=None, pattern_kwargs=None):
```

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.3.3
+Version: 0.3.4
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.3.3/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.3.4/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/setup.cfg` & `pangeo-forge-cordex-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/tests/test_parsing.py` & `pangeo-forge-cordex-0.3.4/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.3.3/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.3.4/tests/test_recipe_creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import xarray as xr
 from pangeo_forge_recipes.patterns import pattern_from_file_sequence
 from pangeo_forge_recipes.recipes import XarrayZarrRecipe
 
 from pangeo_forge_cordex import logon, recipe_inputs_from_iids
 
 iids = [
-    "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
+    #    "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
     "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.mon.tas.v20180813",
 ]
 
 
 @pytest.mark.parametrize("iid", iids)
 def test_recipe_inputs(iid):
     sslcontext = logon()
```

