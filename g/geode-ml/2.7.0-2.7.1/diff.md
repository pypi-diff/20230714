# Comparing `tmp/geode-ml-2.7.0.tar.gz` & `tmp/geode-ml-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geode-ml-2.7.0.tar", last modified: Fri Jul 14 14:29:59 2023, max compression
+gzip compressed data, was "geode-ml-2.7.1.tar", last modified: Fri Jul 14 14:54:44 2023, max compression
```

## Comparing `geode-ml-2.7.0.tar` & `geode-ml-2.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 14:29:59.829506 geode-ml-2.7.0/
--rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.7.0/LICENSE
--rw-rw-rw-   0        0        0     3676 2023-07-14 14:29:59.828503 geode-ml-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1782 2023-07-14 14:25:42.000000 geode-ml-2.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 14:29:59.809054 geode-ml-2.7.0/geode/
--rw-rw-rw-   0        0        0       74 2023-07-14 14:27:11.000000 geode-ml-2.7.0/geode/__init__.py
--rw-rw-rw-   0        0        0    21111 2023-05-02 21:04:51.000000 geode-ml-2.7.0/geode/datasets.py
--rw-rw-rw-   0        0        0     2522 2023-05-09 16:10:45.000000 geode-ml-2.7.0/geode/losses.py
--rw-rw-rw-   0        0        0    22548 2023-07-14 14:25:16.000000 geode-ml-2.7.0/geode/models.py
--rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.7.0/geode/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:29:59.825508 geode-ml-2.7.0/geode_ml.egg-info/
--rw-rw-rw-   0        0        0     3676 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      981 2023-07-14 14:26:47.000000 geode-ml-2.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 14:29:59.829506 geode-ml-2.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 14:54:44.215800 geode-ml-2.7.1/
+-rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.7.1/LICENSE
+-rw-rw-rw-   0        0        0     3677 2023-07-14 14:54:44.214867 geode-ml-2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1782 2023-07-14 14:25:42.000000 geode-ml-2.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 14:54:44.196831 geode-ml-2.7.1/geode/
+-rw-rw-rw-   0        0        0       74 2023-07-14 14:53:20.000000 geode-ml-2.7.1/geode/__init__.py
+-rw-rw-rw-   0        0        0    21111 2023-05-02 21:04:51.000000 geode-ml-2.7.1/geode/datasets.py
+-rw-rw-rw-   0        0        0     2522 2023-05-09 16:10:45.000000 geode-ml-2.7.1/geode/losses.py
+-rw-rw-rw-   0        0        0    22532 2023-07-14 14:52:08.000000 geode-ml-2.7.1/geode/models.py
+-rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.7.1/geode/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:54:44.211837 geode-ml-2.7.1/geode_ml.egg-info/
+-rw-rw-rw-   0        0        0     3677 2023-07-14 14:54:44.000000 geode-ml-2.7.1/geode_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-14 14:54:44.000000 geode-ml-2.7.1/geode_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:54:44.000000 geode-ml-2.7.1/geode_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-07-14 14:54:44.000000 geode-ml-2.7.1/geode_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 14:54:44.000000 geode-ml-2.7.1/geode_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      982 2023-07-14 14:53:38.000000 geode-ml-2.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 14:54:44.215800 geode-ml-2.7.1/setup.cfg
```

### Comparing `geode-ml-2.7.0/LICENSE` & `geode-ml-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geode-ml-2.7.0/PKG-INFO` & `geode-ml-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.7.0
-Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
+Version: 2.7.1
+Summary: Classes and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `geode-ml-2.7.0/README.md` & `geode-ml-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `geode-ml-2.7.0/geode/datasets.py` & `geode-ml-2.7.1/geode/datasets.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.7.0/geode/losses.py` & `geode-ml-2.7.1/geode/losses.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.7.0/geode/models.py` & `geode-ml-2.7.1/geode/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
         Raises:
             Exception: if there are no predicted rasters at test_predictions_path;
         """
 
         # coerce arguments to correct type
         output_path = str(output_path)
-        pos_label = int(pos_label)
         verbose = bool(verbose)
 
         # check that there are predictions
         if len(listdir(self.test_predictions_path)) == 0:
             raise Exception("No predicted imagery has been generated.")
 
         # create dictionary to hold metric dictionaries
@@ -104,16 +103,16 @@
 
             # loop through the test subset
             for fname in sub_filenames:
                 if verbose:
                     print(fname)
 
                 # open the relevant datasets
-                y_true = Open(join(self.test_labels_path, fname)).ReadAsArray()
-                y_pred = Open(join(self.test_predictions_path, fname)).ReadAsArray()
+                y_true = Open(join(self.test_labels_path, fname)).ReadAsArray().flatten()
+                y_pred = Open(join(self.test_predictions_path, fname)).ReadAsArray().flatten()
 
                 # compute metrics
                 f1_scores.append(f1_score(y_true=y_true,
                                           y_pred=y_pred))
 
                 jaccard_scores.append(jaccard_score(y_true=y_true,
                                                     y_pred=y_pred))
```

### Comparing `geode-ml-2.7.0/geode/utilities.py` & `geode-ml-2.7.1/geode/utilities.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.7.0/geode_ml.egg-info/PKG-INFO` & `geode-ml-2.7.1/geode_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.7.0
-Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
+Version: 2.7.1
+Summary: Classes and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `geode-ml-2.7.0/pyproject.toml` & `geode-ml-2.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'geode-ml'
-version = '2.7.0'
-description = "Clases and methods to help with the creation of geospatial training datasets and deep-learning models."
+version = '2.7.1'
+description = "Classes and methods to help with the creation of geospatial training datasets and deep-learning models."
 readme = 'README.md'
 license = {file='LICENSE'}
 authors = [
     {name = 'Matt Reichenbach', email='matthew.reichenbach@gmail.com'},
 ]
 requires-python = '>=3.7'
 classifiers = [
```

