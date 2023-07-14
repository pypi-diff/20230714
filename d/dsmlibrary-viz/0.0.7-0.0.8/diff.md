# Comparing `tmp/dsmlibrary_viz-0.0.7.tar.gz` & `tmp/dsmlibrary_viz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary_viz-0.0.7.tar", last modified: Fri Jul 14 06:23:30 2023, max compression
+gzip compressed data, was "dsmlibrary_viz-0.0.8.tar", last modified: Fri Jul 14 06:45:44 2023, max compression
```

## Comparing `dsmlibrary_viz-0.0.7.tar` & `dsmlibrary_viz-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.476266 dsmlibrary_viz-0.0.7/
--rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.7/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:23:30.475580 dsmlibrary_viz-0.0.7/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      368 2023-07-14 05:57:14.000000 dsmlibrary_viz-0.0.7/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.468950 dsmlibrary_viz-0.0.7/dsmlibrary_viz/
--rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-14 06:23:22.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/base.py
--rw-r--r--   0 naii       (501) staff       (20)     2221 2023-07-13 09:19:09.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/data_viz.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.474403 dsmlibrary_viz-0.0.7/dsmlibrary_viz/scripts/
--rw-r--r--   0 naii       (501) staff       (20)       25 2023-07-14 06:11:01.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/scripts/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      122 2023-07-14 06:21:45.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/scripts/install_ext.py
--rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/utils.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.472397 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      389 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       39 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-14 06:23:30.476477 dsmlibrary_viz-0.0.7/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     2005 2023-07-14 06:22:36.000000 dsmlibrary_viz-0.0.7/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:45:44.379068 dsmlibrary_viz-0.0.8/
+-rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.8/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:45:44.378562 dsmlibrary_viz-0.0.8/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      368 2023-07-14 05:57:14.000000 dsmlibrary_viz-0.0.8/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:45:44.370826 dsmlibrary_viz-0.0.8/dsmlibrary_viz/
+-rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-14 06:45:31.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     2167 2023-07-14 06:45:08.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz/data_viz.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:45:44.377259 dsmlibrary_viz-0.0.8/dsmlibrary_viz/scripts/
+-rw-r--r--   0 naii       (501) staff       (20)       25 2023-07-14 06:11:01.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz/scripts/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      133 2023-07-14 06:33:26.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz/scripts/install_ext.py
+-rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz/utils.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:45:44.375306 dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:45:44.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      389 2023-07-14 06:45:44.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-14 06:45:44.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       39 2023-07-14 06:45:44.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-14 06:45:44.000000 dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-14 06:45:44.379232 dsmlibrary_viz-0.0.8/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     2434 2023-07-14 06:34:30.000000 dsmlibrary_viz-0.0.8/setup.py
```

### Comparing `dsmlibrary_viz-0.0.7/LICENSE` & `dsmlibrary_viz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.7/PKG-INFO` & `dsmlibrary_viz-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary_viz
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.7/dsmlibrary_viz/base.py` & `dsmlibrary_viz-0.0.8/dsmlibrary_viz/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.7/dsmlibrary_viz/data_viz.py` & `dsmlibrary_viz-0.0.8/dsmlibrary_viz/data_viz.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 import duckdb
 from . import base
 import pandas as pd
 
 class DataViz(base.Base):
     
     def __init__(self, token=None, verbose=True, dataplatform_api_uri=None, object_storage_uri=None, apikey=None):
-        try:
-            duckdb.sql("install 'httpfs';")
-        except Exception as e:
-            pass
+        duckdb.sql("install 'httpfs';")
         super().__init__(token, verbose, dataplatform_api_uri, object_storage_uri, apikey)
 
     def _find_fileID(self, match):
         match = match.group()
         _file_id = match.split(':')[-1]
         meta = self.get_meta_file(file_id=_file_id)
         osd_key = meta.get('s3_key')
@@ -49,15 +46,16 @@
             re.sub("DISCOVERY:\d*", self._find_fileID, query),
             re.sub("DISCOVERY:\d*", self._find_fileID2, query),
             re.sub("DISCOVERY:\d*", self._find_fileID3, query)
         ]
 
     def query(self, query_str):
         querys = self._query(query_str)
+        err = None
         for query in querys:
             try:
                 output = duckdb.sql(query).to_df()
             except Exception as e:
-                pass
+                err = e
             else:
                 return output
-        return pd.DataFrame()
+        return err
```

### Comparing `dsmlibrary_viz-0.0.7/dsmlibrary_viz/utils.py` & `dsmlibrary_viz-0.0.8/dsmlibrary_viz/utils.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/PKG-INFO` & `dsmlibrary_viz-0.0.8/dsmlibrary_viz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary-viz
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.7/setup.py` & `dsmlibrary_viz-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,27 +13,37 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 from setuptools.command.develop import develop
 from setuptools.command.install import install
+from setuptools.command.egg_info import egg_info
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
     def run(self):
         develop.run(self)
         scripts.install_ext.install_ext()
+        os.system("echo 'Installed duckdb httpfs done!'")
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         scripts.install_ext.install_ext()
+        os.system("echo 'Installed duckdb httpfs done!'")
+
+class EggInfoCommand(egg_info):
+    """Post-installation for installation mode."""
+    def run(self):
+        egg_info.run(self)
+        scripts.install_ext.install_ext()
+        os.system("echo 'Installed duckdb httpfs done!'")
 
 setup(
     name='dsmlibrary_viz',
     version=get_version(),
     url='https://github.com/storemesh/dsmlibrary-viz',
     packages=find_packages(),
     include_package_data=True,
@@ -60,9 +70,10 @@
         'duckdb',
         'pandas',
         'matplotlib'
     ],
     cmdclass={
         'develop': PostDevelopCommand,
         'install': PostInstallCommand,
+        'egg_info':EggInfoCommand
     }
 )
```

