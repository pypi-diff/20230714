# Comparing `tmp/saracendb-0.7.tar.gz` & `tmp/saracendb-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.7.tar", last modified: Fri Jul 14 10:33:46 2023, max compression
+gzip compressed data, was "saracendb-0.7.1.tar", last modified: Fri Jul 14 10:46:26 2023, max compression
```

## Comparing `saracendb-0.7.tar` & `saracendb-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:33:46.197028 saracendb-0.7/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-14 10:33:46.196899 saracendb-0.7/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.7/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:33:46.196073 saracendb-0.7/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)    10986 2023-07-14 10:32:44.000000 saracendb-0.7/saracendb/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:33:46.196702 saracendb-0.7/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-14 10:33:46.197063 saracendb-0.7/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-14 10:33:11.000000 saracendb-0.7/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:46:26.567581 saracendb-0.7.1/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4536 2023-07-14 10:46:26.567452 saracendb-0.7.1/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.7.1/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:46:26.566610 saracendb-0.7.1/saracendb/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)    11316 2023-07-14 10:45:58.000000 saracendb-0.7.1/saracendb/__init__.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:46:26.567279 saracendb-0.7.1/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4536 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-14 10:46:26.000000 saracendb-0.7.1/saracendb.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-14 10:46:26.567614 saracendb-0.7.1/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      925 2023-07-14 10:46:07.000000 saracendb-0.7.1/setup.py
```

### Comparing `saracendb-0.7/PKG-INFO` & `saracendb-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.7
+Version: 0.7.1
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.7/README.md` & `saracendb-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `saracendb-0.7/saracendb/__init__.py` & `saracendb-0.7.1/saracendb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -207,36 +207,43 @@
     def compact(self) -> None:
         """Remove deleted entries from the database / reduce file size."""
         temp_filename = self.__filename + '.tmp'
         with open(temp_filename, 'wb') as f:
             f.write(bson.encode(self.__data))
         shutil.move(temp_filename, self.__filename)
 
-    def to_json(self, coll: str=None) -> None:
+    def to_json(self, coll: str=None, cust_path: str=None) -> None:
         """Write the collection to a JSON file. If no collection is specified the entire db will be written to the file"""
-        data = ''
-        if not coll:
+        data, file_path = ''
+        if not coll or coll == '':
             coll = 'db'
             data = self.__data
         else:
             data = self.__data[coll]
-        with open(f'{coll}.json', 'w') as f:
-            json.dump(data, f)  
-
+        if cust_path is None:
+            file_path = f'{coll}.json'
+        else:
+            file_path = cust_path
+            with open(file_path, 'w') as f:
+                json.dump(data, f)  
 
-    def to_yaml(self, coll: str=None) -> None:
+    def to_yaml(self, coll: str=None, cust_path: str=None) -> None:
         """Write the collection to a YAML file. If no collection is specified the entire db will be written to the file"""
-        data = ''
-        if not coll:
+        data, file_path = ''
+        if not coll or coll == '':
             coll = 'db'
             data = self.__data
         else:
             data = self.__data[coll]
-        with open(f'{coll}.yaml', 'w') as f:
-            yaml.dump(data, f)  
+        if cust_path is None:
+            file_path = f'{coll}.yaml'
+        else:
+            file_path = cust_path
+            with open(file_path, 'w') as f:
+                yaml.dump(data, f) 
 
     def add_json(self, path: str) -> None:
         """add a JSON file to the current collection."""
         with open(path, 'r') as f:
             file = json.load(f)
         if not isinstance(file, list):
             raise TypeError('File must be of type list.')
```

### Comparing `saracendb-0.7/saracendb.egg-info/PKG-INFO` & `saracendb-0.7.1/saracendb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.7
+Version: 0.7.1
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.7/setup.py` & `saracendb-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.7'
+VERSION = '0.7.1'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
```

