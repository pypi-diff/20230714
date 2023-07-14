# Comparing `tmp/kirkwoodnight-1.0.0.tar.gz` & `tmp/kirkwoodnight-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-1.0.0.tar", last modified: Fri Jul 14 03:10:06 2023, max compression
+gzip compressed data, was "kirkwoodnight-1.0.1.tar", last modified: Fri Jul 14 03:13:22 2023, max compression
```

## Comparing `kirkwoodnight-1.0.0.tar` & `kirkwoodnight-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.870000 kirkwoodnight-1.0.0/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.0/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:10:06.869439 kirkwoodnight-1.0.0/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     4560 2023-07-13 00:00:36.000000 kirkwoodnight-1.0.0/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.860569 kirkwoodnight-1.0.0/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.0/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.0/kirkwoodnight/command_line.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.868528 kirkwoodnight-1.0.0/kirkwoodnight/data/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.0/kirkwoodnight/data/obj_list.csv
--rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.0/kirkwoodnight/plotting.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 02:43:02.000000 kirkwoodnight-1.0.0/kirkwoodnight/source.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.867718 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 03:10:06.870205 kirkwoodnight-1.0.0/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 03:09:51.000000 kirkwoodnight-1.0.0/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.322105 kirkwoodnight-1.0.1/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.1/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:13:22.321600 kirkwoodnight-1.0.1/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4560 2023-07-13 00:00:36.000000 kirkwoodnight-1.0.1/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.315791 kirkwoodnight-1.0.1/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.1/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.1/kirkwoodnight/command_line.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.320799 kirkwoodnight-1.0.1/kirkwoodnight/data/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.1/kirkwoodnight/data/obj_list.csv
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.1/kirkwoodnight/plotting.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 02:43:02.000000 kirkwoodnight-1.0.1/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.320114 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 03:13:22.322317 kirkwoodnight-1.0.1/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 03:13:08.000000 kirkwoodnight-1.0.1/setup.py
```

### Comparing `kirkwoodnight-1.0.0/LICENSE.txt` & `kirkwoodnight-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.0/PKG-INFO` & `kirkwoodnight-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-1.0.0/README.md` & `kirkwoodnight-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.0/kirkwoodnight/command_line.py` & `kirkwoodnight-1.0.1/kirkwoodnight/command_line.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.0/kirkwoodnight/data/obj_list.csv` & `kirkwoodnight-1.0.1/kirkwoodnight/data/obj_list.csv`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.0/kirkwoodnight/plotting.py` & `kirkwoodnight-1.0.1/kirkwoodnight/plotting.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.0/kirkwoodnight/source.py` & `kirkwoodnight-1.0.1/kirkwoodnight/source.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.0/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-1.0.1/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-1.0.0/setup.py` & `kirkwoodnight-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
```

