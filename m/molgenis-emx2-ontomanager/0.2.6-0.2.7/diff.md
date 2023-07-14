# Comparing `tmp/molgenis-emx2-ontomanager-0.2.6.tar.gz` & `tmp/molgenis-emx2-ontomanager-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis-emx2-ontomanager-0.2.6.tar", last modified: Mon Jul 10 14:36:51 2023, max compression
+gzip compressed data, was "molgenis-emx2-ontomanager-0.2.7.tar", last modified: Fri Jul 14 12:55:37 2023, max compression
```

## Comparing `molgenis-emx2-ontomanager-0.2.6.tar` & `molgenis-emx2-ontomanager-0.2.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.179127 molgenis-emx2-ontomanager-0.2.6/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6676 2023-07-10 14:36:51.178794 molgenis-emx2-ontomanager-0.2.6/PKG-INFO
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6152 2023-07-07 07:34:04.000000 molgenis-emx2-ontomanager-0.2.6/README.md
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.169239 molgenis-emx2-ontomanager-0.2.6/demos/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.170624 molgenis-emx2-ontomanager-0.2.6/demos/data/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-05 10:52:46.000000 molgenis-emx2-ontomanager-0.2.6/demos/data/Countries.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-03 12:58:30.000000 molgenis-emx2-ontomanager-0.2.6/demos/data/update.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2279 2023-07-05 14:32:26.000000 molgenis-emx2-ontomanager-0.2.6/demos/demo_csv_upload.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2150 2023-07-05 10:54:36.000000 molgenis-emx2-ontomanager-0.2.6/demos/demo_ontomanager.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1860 2023-07-05 08:54:51.000000 molgenis-emx2-ontomanager-0.2.6/demos/demo_search.py
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.172142 molgenis-emx2-ontomanager-0.2.6/dev/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.173235 molgenis-emx2-ontomanager-0.2.6/dev/data/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-05 10:52:46.000000 molgenis-emx2-ontomanager-0.2.6/dev/data/Countries.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-03 12:58:30.000000 molgenis-emx2-ontomanager-0.2.6/dev/data/update.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2322 2023-07-05 14:50:19.000000 molgenis-emx2-ontomanager-0.2.6/dev/dev_csv_upload.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2413 2023-07-07 08:44:17.000000 molgenis-emx2-ontomanager-0.2.6/dev/dev_ontomanager.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1692 2023-07-07 09:46:26.000000 molgenis-emx2-ontomanager-0.2.6/dev/dev_search.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      752 2023-07-10 14:33:54.000000 molgenis-emx2-ontomanager-0.2.6/pyproject.toml
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       97 2023-07-10 13:14:26.000000 molgenis-emx2-ontomanager-0.2.6/requirements.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2023-07-10 14:36:51.179204 molgenis-emx2-ontomanager-0.2.6/setup.cfg
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.165012 molgenis-emx2-ontomanager-0.2.6/src/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.176464 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)    22093 2023-07-10 14:31:20.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/OntologyManager.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       60 2023-06-28 11:55:29.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/__init__.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3500 2023-06-28 13:26:24.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/__main__.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-03 08:33:42.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/cli.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      127 2023-06-28 11:55:29.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/constants.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1445 2023-07-03 14:40:41.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/exceptions.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3729 2023-07-03 09:45:28.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/graphql_queries.py
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-10 14:36:51.178350 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6676 2023-07-10 14:36:50.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      848 2023-07-10 14:36:51.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        1 2023-07-10 14:36:50.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/dependency_links.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       98 2023-07-10 14:36:50.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/requires.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       26 2023-07-10 14:36:50.000000 molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/top_level.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        5 2023-07-10 14:33:54.000000 molgenis-emx2-ontomanager-0.2.6/version.txt
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:37.013310 molgenis-emx2-ontomanager-0.2.7/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6582 2023-07-14 12:55:37.012858 molgenis-emx2-ontomanager-0.2.7/PKG-INFO
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6058 2023-07-12 10:49:23.000000 molgenis-emx2-ontomanager-0.2.7/README.md
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:36.998303 molgenis-emx2-ontomanager-0.2.7/demos/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:37.000453 molgenis-emx2-ontomanager-0.2.7/demos/data/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-05 10:52:46.000000 molgenis-emx2-ontomanager-0.2.7/demos/data/Countries.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-03 12:58:30.000000 molgenis-emx2-ontomanager-0.2.7/demos/data/update.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2279 2023-07-05 14:32:26.000000 molgenis-emx2-ontomanager-0.2.7/demos/demo_csv_upload.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2150 2023-07-05 10:54:36.000000 molgenis-emx2-ontomanager-0.2.7/demos/demo_ontomanager.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1860 2023-07-05 08:54:51.000000 molgenis-emx2-ontomanager-0.2.7/demos/demo_search.py
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:37.002746 molgenis-emx2-ontomanager-0.2.7/dev/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:37.004018 molgenis-emx2-ontomanager-0.2.7/dev/data/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-05 10:52:46.000000 molgenis-emx2-ontomanager-0.2.7/dev/data/Countries.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-03 12:58:30.000000 molgenis-emx2-ontomanager-0.2.7/dev/data/update.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2322 2023-07-05 14:50:19.000000 molgenis-emx2-ontomanager-0.2.7/dev/dev_csv_upload.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2414 2023-07-12 14:24:23.000000 molgenis-emx2-ontomanager-0.2.7/dev/dev_ontomanager.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1882 2023-07-14 08:50:25.000000 molgenis-emx2-ontomanager-0.2.7/dev/dev_search.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      752 2023-07-10 14:33:54.000000 molgenis-emx2-ontomanager-0.2.7/pyproject.toml
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       97 2023-07-10 13:14:26.000000 molgenis-emx2-ontomanager-0.2.7/requirements.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2023-07-14 12:55:37.013426 molgenis-emx2-ontomanager-0.2.7/setup.cfg
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:36.993502 molgenis-emx2-ontomanager-0.2.7/src/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:37.009125 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)    22983 2023-07-14 12:54:25.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/OntologyManager.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       60 2023-06-28 11:55:29.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/__init__.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3500 2023-06-28 13:26:24.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/__main__.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-03 08:33:42.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/cli.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      127 2023-06-28 11:55:29.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/constants.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1445 2023-07-03 14:40:41.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/exceptions.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3729 2023-07-03 09:45:28.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/graphql_queries.py
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-14 12:55:37.012073 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6582 2023-07-14 12:55:36.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      848 2023-07-14 12:55:36.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        1 2023-07-14 12:55:36.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       98 2023-07-14 12:55:36.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/requires.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       26 2023-07-14 12:55:36.000000 molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/top_level.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        5 2023-07-14 12:08:27.000000 molgenis-emx2-ontomanager-0.2.7/version.txt
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/PKG-INFO` & `molgenis-emx2-ontomanager-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-ontomanager
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tool to manage catalogue ontologies on Molgenis EMX2 servers.
 Project-URL: Homepage, https://github.com/molgenis/molgenis-emx2
 Project-URL: Bug Tracker, https://github.com/molgenis/molgenis-emx2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -35,32 +35,25 @@
 Set up the virtual environment and install the required packages
 
     python3 -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
 
 #### Building the package
-Specify the version in `pyproject.toml`
-    
-    ...
-    [project]
-    name = "molgenis-emx2-ontomanager"
-    version = "x.y.z"
-    description = "Tool to manage catalogue ontologies on Molgenis EMX2 servers."
-    ...
+Specify the package version by creating the `version.txt` file and writing the version number on the first line of this file. 
 
 
 Build the package
 
     python3 -m build
 
 Install the built package
 
     pip install dist/molgenis-emx2-ontomanager-x.y.z-py3-none-any.whl
-where `x.y.z` is the version you set in the `pyproject.toml` file.
+where `x.y.z` is the version you set in the `version.txt` file.
 
 
 ## How to use
 
 ### In Python scripts
 Import the OntologyManager class from the package and create an instance by providing login details.
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/README.md` & `molgenis-emx2-ontomanager-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,25 @@
 Set up the virtual environment and install the required packages
 
     python3 -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
 
 #### Building the package
-Specify the version in `pyproject.toml`
-    
-    ...
-    [project]
-    name = "molgenis-emx2-ontomanager"
-    version = "x.y.z"
-    description = "Tool to manage catalogue ontologies on Molgenis EMX2 servers."
-    ...
+Specify the package version by creating the `version.txt` file and writing the version number on the first line of this file. 
 
 
 Build the package
 
     python3 -m build
 
 Install the built package
 
     pip install dist/molgenis-emx2-ontomanager-x.y.z-py3-none-any.whl
-where `x.y.z` is the version you set in the `pyproject.toml` file.
+where `x.y.z` is the version you set in the `version.txt` file.
 
 
 ## How to use
 
 ### In Python scripts
 Import the OntologyManager class from the package and create an instance by providing login details.
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/demos/demo_csv_upload.py` & `molgenis-emx2-ontomanager-0.2.7/demos/demo_csv_upload.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/demos/demo_ontomanager.py` & `molgenis-emx2-ontomanager-0.2.7/demos/demo_ontomanager.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/demos/demo_search.py` & `molgenis-emx2-ontomanager-0.2.7/demos/demo_search.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/dev/dev_csv_upload.py` & `molgenis-emx2-ontomanager-0.2.7/dev/dev_csv_upload.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/dev/dev_ontomanager.py` & `molgenis-emx2-ontomanager-0.2.7/dev/dev_ontomanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,11 +55,11 @@
 
     # manager.delete(table='Countries', name="Armadilland")
     # manager.delete(table='Countries', name="Republic of Molgenia")
     # manager.delete(table='Countries', names=["Armadilland", "Republic of Molgenia"])
 
 
 if __name__ == '__main__':
-    logging.basicConfig(level='INFO')
+    logging.basicConfig(level='DEBUG')
     logging.getLogger("requests").setLevel(logging.WARNING)
     logging.getLogger("urllib3").setLevel(logging.WARNING)
     dev_ontomanager()
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/dev/dev_search.py` & `molgenis-emx2-ontomanager-0.2.7/dev/dev_search.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 MG_URL = https://myserver.molgeniscloud.org
 MG_USERNAME = username
 MG_PASSWORD = password
 
 Ensure the CatalogueOntologies database is present on the server before running the script.
 """
+import logging
 import os
 
 from dotenv import load_dotenv
 
 from tools.ontomanager.src.molgenis_emx2_ontomanager import OntologyManager
 
 
@@ -35,18 +36,21 @@
     if isinstance(search_terms, str):
         search_terms = list(search_terms)
     if not isinstance(search_terms, list):
         raise ValueError("Supply the search terms as a string or a list.")
 
     results = dict()
     for st in search_terms:
-        _table = manager.search(st)
+        _table = manager.search(st, find_usage=True)
         results[st] = _table
 
     return results
 
 
 if __name__ == '__main__':
+    logging.basicConfig(level='DEBUG')
+    logging.getLogger("requests").setLevel(logging.WARNING)
+    logging.getLogger("urllib3").setLevel(logging.WARNING)
     terms = ['Sibling', 'Croatia', 'Non-profit organisations', 'Hospital data', 'medication']
     demo_results = dev_search(terms)
     for (term, table) in demo_results.items():
         print(f"{term}: {table}")
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/pyproject.toml` & `molgenis-emx2-ontomanager-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/OntologyManager.py` & `molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/OntologyManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         :param url: the URL to the server
         :param username: the username to sign in to the server
         :param password: the password that belongs to the username for this server
         """
         self.client = Client(url=url, username=username, password=password)
         self.graphql_endpoint = f'{self.client.url}/CatalogueOntologies/graphql'
         self.ontology_tables = self.__list_ontology_tables()
+        self.schema = self.get_schema()
 
         if self.client.signin_status == 'failed':
             self.client.session.close()
             raise SigninError('Signing in failed. Exiting.')
 
     def perform(self, action: str, table: str, **kwargs):
         """Select the method to perform and pass any keyword arguments"""
@@ -142,28 +143,30 @@
             return {table: usage}
 
         return table
 
     def _search_usage(self, term: str, ontology_table: str) -> dict | None:
         """Search for the ontology term's usage in all databases on the server."""
         usage_dict = dict()
-        for db in self.list_databases():
-            try:
-                db_schema = self.get_database_schema(db)
-            except InvalidDatabaseException:
-                continue
-            db_dict = dict()
+        for db, db_schema in self.schema.items():
+            db_usage_dict = dict()
             for tb_name, tb_values in db_schema.items():
                 if tb_values.get('externalSchema') != db:
                     continue
                 for col_name, col_values in tb_values['columns'].items():
                     if not (col_values.get('refSchema') == 'CatalogueOntologies'
                             and col_values.get('refTable') == ontology_table):
                         continue
-                    tb_pkeys = [col for (col, col_values) in tb_values['columns'].items() if col_values.get('key') == 1]
+
+                    tb_pkeys = [
+                        (col if col_vals.get('columnType') != 'REF'
+                         else col + ' {' + (", ".join(c for (c, v) in db_schema[col_vals['refTable']]['columns'].items()
+                                                      if v.get('key') == 1)) + '}')
+                        for (col, col_vals) in tb_values['columns'].items() if col_vals.get('key') == 1
+                    ]
                     _table = self.parse_table_name(tb_name)
                     query = Queries.column_values(_table, self.parse_column_name(col_name), tb_pkeys)
                     variables = {'filter': {self.parse_column_name(col_name): {'equals': {'name': term}}}}
 
                     response = self.client.session.post(
                         f'{self.client.url}/{db}/graphql',
                         json={'query': query, 'variables': variables}
@@ -171,17 +174,17 @@
                     if response.status_code != 200:
                         log.error(response.json()['errors'])
                         continue
                     if len(response.json()['data']) == 0:
                         continue
 
                     column_values = response.json()['data'][_table]
-                    db_dict.update({tb_name: column_values})
-            if len(db_dict.keys()) > 0:
-                usage_dict.update({db: db_dict})
+                    db_usage_dict.update({tb_name: column_values})
+            if len(db_usage_dict.keys()) > 0:
+                usage_dict.update({db: db_usage_dict})
         return usage_dict
 
     def _add_term(self, table: str, kwargs):
         """Add a single term to a table."""
 
         _kwargs = self.__parse_kwargs(kwargs)
         _table = self.parse_table_name(table)
@@ -297,15 +300,15 @@
         return response
 
     class Updater:
         """Class that handles the update of the terms, ontology tables, databases and database tables."""
 
         def __init__(self, manager, ontology_table: str, old: str, new: str):
             self.ontology_table = ontology_table
-            self.manager = manager
+            self.manager: OntologyManager = manager
             self.old = old
             self.new = new
 
             self.database = None
             self.table = None
             self.column = None
 
@@ -325,15 +328,15 @@
 
         def __update_database(self, database: str) -> dict:
             """Update the tables in the database, replacing the 'old' term with the 'new' term.
             :param database: the name of the database
             """
             db_dict = dict()
             try:
-                db_schema = self.manager.get_database_schema(database)
+                db_schema = self.manager.schema.get(database)
             except InvalidDatabaseException:
                 return db_dict
 
             for tb_name, tb_values in db_schema.items():
                 self.table = tb_name
                 if tb_values.get('externalSchema') != database:
                     continue
@@ -346,15 +349,22 @@
 
         def __update_table(self, tb_name: str, tb_values: dict) -> dict:
             """
             Update a data table in the database.
             """
             tb_dict = dict()
 
-            tb_pkeys = [col for (col, col_values) in tb_values['columns'].items() if col_values.get('key') == 1]
+            # tb_pkeys = [col for (col, col_values) in tb_values['columns'].items() if col_values.get('key') == 1]
+
+            tb_pkeys = [
+                (col if col_vals.get('columnType') != 'REF'
+                 else col + ' {' + (", ".join(c for (c, v) in self.manager.schema[self.database][col_vals['refTable']]['columns'].items()
+                                              if v.get('key') == 1)) + '}')
+                for (col, col_vals) in tb_values['columns'].items() if col_vals.get('key') == 1
+            ]
 
             for col, col_values in tb_values['columns'].items():
                 self.column = col
                 if not (col_values.get('refSchema') == 'CatalogueOntologies'
                         and col_values.get('refTable') == self.ontology_table):
                     continue
                 col_dict = self.__update_column(tb_pkeys)
@@ -466,14 +476,22 @@
         response = self.client.session.post(
             url=f'{self.client.url}/apps/graphql',
             json={"query": query}
         )
         databases = [db['name'] for db in response.json()['data']['_schemas']]
         return databases
 
+    def get_schema(self):
+        """Get the schema for all databases on the server."""
+        schema = {
+            db: self.get_database_schema(db)
+            for db in self.list_databases()
+        }
+        return schema
+
     def get_database_schema(self, database: str) -> dict:
         """Returns the schema of the specified database.
         :param database: the name of the database.
         """
         query = Queries.database_schema()
         response = self.client.session.post(
             url=f'{self.client.url}/{database}/graphql',
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/__main__.py` & `molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/__main__.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/exceptions.py` & `molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager/graphql_queries.py` & `molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO` & `molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-ontomanager
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tool to manage catalogue ontologies on Molgenis EMX2 servers.
 Project-URL: Homepage, https://github.com/molgenis/molgenis-emx2
 Project-URL: Bug Tracker, https://github.com/molgenis/molgenis-emx2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -35,32 +35,25 @@
 Set up the virtual environment and install the required packages
 
     python3 -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
 
 #### Building the package
-Specify the version in `pyproject.toml`
-    
-    ...
-    [project]
-    name = "molgenis-emx2-ontomanager"
-    version = "x.y.z"
-    description = "Tool to manage catalogue ontologies on Molgenis EMX2 servers."
-    ...
+Specify the package version by creating the `version.txt` file and writing the version number on the first line of this file. 
 
 
 Build the package
 
     python3 -m build
 
 Install the built package
 
     pip install dist/molgenis-emx2-ontomanager-x.y.z-py3-none-any.whl
-where `x.y.z` is the version you set in the `pyproject.toml` file.
+where `x.y.z` is the version you set in the `version.txt` file.
 
 
 ## How to use
 
 ### In Python scripts
 Import the OntologyManager class from the package and create an instance by providing login details.
```

### Comparing `molgenis-emx2-ontomanager-0.2.6/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt` & `molgenis-emx2-ontomanager-0.2.7/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

