# Comparing `tmp/hashlistdict-0.10.tar.gz` & `tmp/hashlistdict-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashlistdict-0.10.tar", last modified: Thu Jul 13 21:43:19 2023, max compression
+gzip compressed data, was "hashlistdict-0.11.tar", last modified: Fri Jul 14 15:05:07 2023, max compression
```

## Comparing `hashlistdict-0.10.tar` & `hashlistdict-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 21:43:19.336068 hashlistdict-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-13 21:43:08.000000 hashlistdict-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      107 2023-07-13 21:43:02.000000 hashlistdict-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     6151 2023-07-13 21:43:19.336068 hashlistdict-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     5408 2023-07-13 21:39:55.000000 hashlistdict-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 21:43:19.333078 hashlistdict-0.10/hashlistdict/
--rw-rw-rw-   0        0        0     5408 2023-07-13 21:39:55.000000 hashlistdict-0.10/hashlistdict/README.MD
--rw-rw-rw-   0        0        0     1906 2023-07-13 21:29:53.000000 hashlistdict-0.10/hashlistdict/__init__.py
--rw-rw-rw-   0        0        0       39 2023-07-13 21:43:18.000000 hashlistdict-0.10/hashlistdict/requirements.txt
--rw-rw-rw-   0        0        0     1277 2023-07-13 21:43:18.000000 hashlistdict-0.10/hashlistdict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-13 21:43:19.335071 hashlistdict-0.10/hashlistdict.egg-info/
--rw-rw-rw-   0        0        0     6151 2023-07-13 21:43:19.000000 hashlistdict-0.10/hashlistdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-07-13 21:43:19.000000 hashlistdict-0.10/hashlistdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 21:43:19.000000 hashlistdict-0.10/hashlistdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-13 21:43:19.000000 hashlistdict-0.10/hashlistdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 21:43:19.000000 hashlistdict-0.10/hashlistdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-13 21:43:19.338064 hashlistdict-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1470 2023-07-13 21:43:18.000000 hashlistdict-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:05:07.816918 hashlistdict-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-14 15:05:00.000000 hashlistdict-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      107 2023-07-14 15:04:59.000000 hashlistdict-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     6151 2023-07-14 15:05:07.816918 hashlistdict-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     5408 2023-07-13 21:39:55.000000 hashlistdict-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:05:07.813926 hashlistdict-0.11/hashlistdict/
+-rw-rw-rw-   0        0        0     5408 2023-07-13 21:39:55.000000 hashlistdict-0.11/hashlistdict/README.MD
+-rw-rw-rw-   0        0        0     1554 2023-07-14 15:03:42.000000 hashlistdict-0.11/hashlistdict/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-07-14 15:05:06.000000 hashlistdict-0.11/hashlistdict/requirements.txt
+-rw-rw-rw-   0        0        0     1277 2023-07-14 15:05:06.000000 hashlistdict-0.11/hashlistdict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-14 15:05:07.816918 hashlistdict-0.11/hashlistdict.egg-info/
+-rw-rw-rw-   0        0        0     6151 2023-07-14 15:05:07.000000 hashlistdict-0.11/hashlistdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-07-14 15:05:07.000000 hashlistdict-0.11/hashlistdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:05:07.000000 hashlistdict-0.11/hashlistdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 15:05:07.000000 hashlistdict-0.11/hashlistdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 15:05:07.000000 hashlistdict-0.11/hashlistdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-14 15:05:07.818913 hashlistdict-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1470 2023-07-14 15:05:06.000000 hashlistdict-0.11/setup.py
```

### Comparing `hashlistdict-0.10/LICENSE.rst` & `hashlistdict-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hashlistdict-0.10/PKG-INFO` & `hashlistdict-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashlistdict
-Version: 0.10
+Version: 0.11
 Summary: Hashable dict/list - subclasses of list/dict with a custom hash function based on alternating addition and subtraction of element hashes - pure Python
 Home-page: https://github.com/hansalemaos/hashlistdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,list,dict,hash,hashable
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hashlistdict-0.10/README.md` & `hashlistdict-0.11/README.md`

 * *Files identical despite different names*

### Comparing `hashlistdict-0.10/hashlistdict/README.MD` & `hashlistdict-0.11/hashlistdict/README.MD`

 * *Files identical despite different names*

### Comparing `hashlistdict-0.10/hashlistdict/__init__.py` & `hashlistdict-0.11/hashlistdict/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,21 +15,16 @@
         l1 = HashList([1, 2, 3, 4, {1: 2, 3: 4}])
         print(hash(l1))
         # Output: -5103430572081493847
 
     """
 
     def __hash__(self):
-        allhashes = 1
-        for ini, f in enumerate(fla_tu(self)):
-            if ini % 2 == 0:
-                allhashes += hash(f)
-            else:
-                allhashes -= hash(f)
-        return allhashes
+        return hash(tuple(fla_tu(self)))+1
+
 
 
 class HashDict(dict):
     """A subclass of dict that provides a custom hash function.
 
     This class overrides the __hash__() method to compute a hash value based on the key-value pairs of the dictionary.
     The hash value is calculated by alternating between adding and subtracting the hash values of the keys and values.
@@ -42,17 +37,11 @@
         d1 = HashDict({1: 'a', 2: 'b', 3: 'c'})
         print(hash(d1))
         # Output: -5076628985615637757
 
     """
 
     def __hash__(self):
-        allhashes = 2
-        for ini, f in enumerate(fla_tu(self)):
-            if ini % 2 == 0:
-                allhashes += hash(f)
-            else:
-                allhashes -= hash(f)
+        return hash(tuple(fla_tu(self))) + 2
 
-        return allhashes
```

### Comparing `hashlistdict-0.10/hashlistdict/thirdparty.json` & `hashlistdict-0.11/hashlistdict/thirdparty.json`

 * *Files identical despite different names*

### Comparing `hashlistdict-0.10/hashlistdict.egg-info/PKG-INFO` & `hashlistdict-0.11/hashlistdict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashlistdict
-Version: 0.10
+Version: 0.11
 Summary: Hashable dict/list - subclasses of list/dict with a custom hash function based on alternating addition and subtraction of element hashes - pure Python
 Home-page: https://github.com/hansalemaos/hashlistdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested,list,dict,hash,hashable
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hashlistdict-0.10/setup.py` & `hashlistdict-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Hashable dict/list - subclasses of list/dict with a custom hash function based on alternating addition and subtraction of element hashes - pure Python'''
 
 # Setting up
 setup(
     name="hashlistdict",
     version=VERSION,
     license='MIT',
```

