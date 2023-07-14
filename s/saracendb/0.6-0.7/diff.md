# Comparing `tmp/saracendb-0.6.tar.gz` & `tmp/saracendb-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.6.tar", last modified: Thu Jul 13 14:50:13 2023, max compression
+gzip compressed data, was "saracendb-0.7.tar", last modified: Fri Jul 14 10:33:46 2023, max compression
```

## Comparing `saracendb-0.6.tar` & `saracendb-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-13 14:50:13.981534 saracendb-0.6/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-13 14:50:13.981395 saracendb-0.6/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.6/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-13 14:50:13.980507 saracendb-0.6/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)    10942 2023-07-13 14:47:19.000000 saracendb-0.6/saracendb/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-13 14:50:13.981212 saracendb-0.6/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-13 14:50:13.981576 saracendb-0.6/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-13 14:47:32.000000 saracendb-0.6/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:33:46.197028 saracendb-0.7/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-14 10:33:46.196899 saracendb-0.7/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.7/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:33:46.196073 saracendb-0.7/saracendb/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)    10986 2023-07-14 10:32:44.000000 saracendb-0.7/saracendb/__init__.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-14 10:33:46.196702 saracendb-0.7/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-14 10:33:46.000000 saracendb-0.7/saracendb.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-14 10:33:46.197063 saracendb-0.7/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-14 10:33:11.000000 saracendb-0.7/setup.py
```

### Comparing `saracendb-0.6/PKG-INFO` & `saracendb-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.6
+Version: 0.7
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.6/README.md` & `saracendb-0.7/README.md`

 * *Files identical despite different names*

### Comparing `saracendb-0.6/saracendb/__init__.py` & `saracendb-0.7/saracendb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,33 +207,36 @@
     def compact(self) -> None:
         """Remove deleted entries from the database / reduce file size."""
         temp_filename = self.__filename + '.tmp'
         with open(temp_filename, 'wb') as f:
             f.write(bson.encode(self.__data))
         shutil.move(temp_filename, self.__filename)
 
-    def to_json(self, path: str='collection.json') -> None:
-        """Write the collection to a JSON file."""
-        with open(path, 'w') as f:
-            json.dump(self.__data[self.__coll], f)
-
-    def to_yaml(self, path: str='collection.yml') -> None:
-        """Write the collection to a YAML file."""
-        with open(path, 'w') as f:
-            yaml.dump(self.__data[self.__coll], f)
-
-    def db_to_json(self, path: str='db.json') -> None:
-        """Write the database to a JSON file."""
-        with open(path, 'w') as f:
-            json.dump(self.__data, f)
-
-    def db_to_yaml(self, path: str='db.yml') -> None:
-        """Write the database to a YAML file."""
-        with open(path, 'w') as f:
-            yaml.dump(self.__data, f)
+    def to_json(self, coll: str=None) -> None:
+        """Write the collection to a JSON file. If no collection is specified the entire db will be written to the file"""
+        data = ''
+        if not coll:
+            coll = 'db'
+            data = self.__data
+        else:
+            data = self.__data[coll]
+        with open(f'{coll}.json', 'w') as f:
+            json.dump(data, f)  
+
+
+    def to_yaml(self, coll: str=None) -> None:
+        """Write the collection to a YAML file. If no collection is specified the entire db will be written to the file"""
+        data = ''
+        if not coll:
+            coll = 'db'
+            data = self.__data
+        else:
+            data = self.__data[coll]
+        with open(f'{coll}.yaml', 'w') as f:
+            yaml.dump(data, f)  
 
     def add_json(self, path: str) -> None:
         """add a JSON file to the current collection."""
         with open(path, 'r') as f:
             file = json.load(f)
         if not isinstance(file, list):
             raise TypeError('File must be of type list.')
@@ -267,15 +270,15 @@
         """Reindex the current collection."""
         for i, entry in enumerate(self.__data[self.__coll]):
             entry['#'] = i
         self.push()
         self.compact()
 
     def get_coll(self) -> None:
-        """Return the current collection."""
+        """Return the current collection data."""
         return self.__data[self.__coll]
     
     def set_coll(self, coll: list) -> None:
         """Overwrite the current collection."""
         if not isinstance(coll, list):
             raise TypeError('Collection must be of type list.')
         self.__data[self.__coll] = coll
```

### Comparing `saracendb-0.6/saracendb.egg-info/PKG-INFO` & `saracendb-0.7/saracendb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saracendb
-Version: 0.6
+Version: 0.7
 Author: Saracen Rhue
 Author-email: 
 Keywords: python,db
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `saracendb-0.6/setup.py` & `saracendb-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.6'
+VERSION = '0.7'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
```

