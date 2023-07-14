# Comparing `tmp/regrez-2.1.8.tar.gz` & `tmp/regrez-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-2.1.8.tar", last modified: Thu Jun 29 13:21:06 2023, max compression
+gzip compressed data, was "regrez-2.1.9.tar", last modified: Fri Jul 14 15:27:53 2023, max compression
```

## Comparing `regrez-2.1.8.tar` & `regrez-2.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:21:06.551483 regrez-2.1.8/
--rw-rw-rw-   0        0        0     2106 2023-06-29 13:21:06.546494 regrez-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1611 2023-06-29 13:16:44.000000 regrez-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 13:21:06.426815 regrez-2.1.8/regrez/
--rw-rw-rw-   0        0        0       28 2023-06-29 12:41:43.000000 regrez-2.1.8/regrez/__init__.py
--rw-rw-rw-   0        0        0     4742 2023-06-29 13:20:47.000000 regrez-2.1.8/regrez/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:21:06.541232 regrez-2.1.8/regrez.egg-info/
--rw-rw-rw-   0        0        0     2106 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:21:06.552495 regrez-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-29 13:20:59.000000 regrez-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:53.932559 regrez-2.1.9/
+-rw-rw-rw-   0        0        0     1940 2023-07-14 15:27:53.931422 regrez-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1504 2023-07-14 15:27:07.000000 regrez-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:53.900602 regrez-2.1.9/regrez/
+-rw-rw-rw-   0        0        0       28 2023-06-29 12:41:43.000000 regrez-2.1.9/regrez/__init__.py
+-rw-rw-rw-   0        0        0     4742 2023-06-29 13:20:47.000000 regrez-2.1.9/regrez/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:53.930918 regrez-2.1.9/regrez.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-07-14 15:27:53.000000 regrez-2.1.9/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-14 15:27:53.000000 regrez-2.1.9/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:27:53.000000 regrez-2.1.9/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 15:27:53.000000 regrez-2.1.9/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 15:27:53.000000 regrez-2.1.9/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:27:53.932559 regrez-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-07-14 15:27:35.000000 regrez-2.1.9/setup.py
```

### Comparing `regrez-2.1.8/PKG-INFO` & `regrez-2.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 2.1.8
+Version: 2.1.9
 Summary: Easiest way to implement linear regression.
-Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
-License: UNKNOWN
 Keywords: regression,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
-This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
+This is a simple Python package that aims to make using linear regression easier for programmers.
 
 You can create a simple linear regression model as following:
 
 ```
 from regrez import Models
 
 m = Models.Simple("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
@@ -30,8 +27,7 @@
 
 ```
 from regrez import Models
 m = Models.Multiple("path/to/csv", ["X Label 1", "X Label 2", "X Label 3"], ["Y Label"])
 ```
 
 After that, you can train your model using `m.Train()` and test using `m.Test(test_x, test_y)`. Alternatively, there is a function called `m.TrainAndTest()` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. There is no `m.Visualize()` for multiple linear regression models.
-
```

### Comparing `regrez-2.1.8/README.md` & `regrez-2.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
+This is a simple Python package that aims to make using linear regression easier for programmers.
 
 You can create a simple linear regression model as following:
 
 ```
 from regrez import Models
 
 m = Models.Simple("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
```

### Comparing `regrez-2.1.8/regrez/main.py` & `regrez-2.1.9/regrez/main.py`

 * *Files identical despite different names*

### Comparing `regrez-2.1.8/regrez.egg-info/PKG-INFO` & `regrez-2.1.9/regrez.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 2.1.8
+Version: 2.1.9
 Summary: Easiest way to implement linear regression.
-Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
-License: UNKNOWN
 Keywords: regression,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
-This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
+This is a simple Python package that aims to make using linear regression easier for programmers.
 
 You can create a simple linear regression model as following:
 
 ```
 from regrez import Models
 
 m = Models.Simple("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
@@ -30,8 +27,7 @@
 
 ```
 from regrez import Models
 m = Models.Multiple("path/to/csv", ["X Label 1", "X Label 2", "X Label 3"], ["Y Label"])
 ```
 
 After that, you can train your model using `m.Train()` and test using `m.Test(test_x, test_y)`. Alternatively, there is a function called `m.TrainAndTest()` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. There is no `m.Visualize()` for multiple linear regression models.
-
```

### Comparing `regrez-2.1.8/setup.py` & `regrez-2.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.1.8' 
+VERSION = '2.1.9' 
 DESCRIPTION = 'Easiest way to implement linear regression.'
 
 with open('README.md') as f:
     long = f.read()
 setup(
         name="regrez", 
         version=VERSION,
```

