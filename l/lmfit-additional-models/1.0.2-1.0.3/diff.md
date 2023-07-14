# Comparing `tmp/lmfit-additional-models-1.0.2.tar.gz` & `tmp/lmfit-additional-models-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lmfit-additional-models-1.0.2.tar", last modified: Fri May 19 09:22:39 2023, max compression
+gzip compressed data, was "dist/lmfit-additional-models-1.0.3.tar", last modified: Fri Jul 14 11:45:09 2023, max compression
```

## Comparing `lmfit-additional-models-1.0.2.tar` & `lmfit-additional-models-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-05-19 09:22:39.495175 lmfit-additional-models-1.0.2/
--rwxrwxrwx   0 julian    (1000) julian    (1000)     1091 2023-05-19 09:22:39.493176 lmfit-additional-models-1.0.2/PKG-INFO
-drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-05-19 09:22:39.489178 lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/
--rwxrwxrwx   0 julian    (1000) julian    (1000)     1091 2023-05-19 09:22:38.000000 lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/PKG-INFO
--rwxrwxrwx   0 julian    (1000) julian    (1000)      242 2023-05-19 09:22:39.000000 lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/SOURCES.txt
--rwxrwxrwx   0 julian    (1000) julian    (1000)        1 2023-05-19 09:22:38.000000 lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/dependency_links.txt
--rwxrwxrwx   0 julian    (1000) julian    (1000)       18 2023-05-19 09:22:39.000000 lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/requires.txt
--rwxrwxrwx   0 julian    (1000) julian    (1000)        1 2023-05-19 09:22:39.000000 lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/top_level.txt
--rwxrwxrwx   0 julian    (1000) julian    (1000)       38 2023-05-19 09:22:39.495175 lmfit-additional-models-1.0.2/setup.cfg
--rwxrwxrwx   0 julian    (1000) julian    (1000)     1298 2023-05-19 09:22:26.000000 lmfit-additional-models-1.0.2/setup.py
+drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-14 11:45:09.645174 lmfit-additional-models-1.0.3/
+-rwxrwxrwx   0 julian    (1000) julian    (1000)     1101 2023-07-14 11:45:09.643173 lmfit-additional-models-1.0.3/PKG-INFO
+drwxrwxrwx   0 julian    (1000) julian    (1000)        0 2023-07-14 11:45:09.641174 lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/
+-rwxrwxrwx   0 julian    (1000) julian    (1000)     1101 2023-07-14 11:45:08.000000 lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/PKG-INFO
+-rwxrwxrwx   0 julian    (1000) julian    (1000)      242 2023-07-14 11:45:09.000000 lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/SOURCES.txt
+-rwxrwxrwx   0 julian    (1000) julian    (1000)        1 2023-07-14 11:45:08.000000 lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/dependency_links.txt
+-rwxrwxrwx   0 julian    (1000) julian    (1000)       18 2023-07-14 11:45:09.000000 lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/requires.txt
+-rwxrwxrwx   0 julian    (1000) julian    (1000)        1 2023-07-14 11:45:09.000000 lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/top_level.txt
+-rwxrwxrwx   0 julian    (1000) julian    (1000)       38 2023-07-14 11:45:09.646172 lmfit-additional-models-1.0.3/setup.cfg
+-rwxrwxrwx   0 julian    (1000) julian    (1000)     1312 2023-07-14 11:44:54.000000 lmfit-additional-models-1.0.3/setup.py
```

### Comparing `lmfit-additional-models-1.0.2/PKG-INFO` & `lmfit-additional-models-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: lmfit-additional-models
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package contains additional models for the lmfit package.
 Author: Julian Hochhaus
 Author-email: julian.hochhaus@tu-dortmund.de
 Description-Content-Type: text/markdown
 
-# lmfit-additional-models 
+# lmfit-additional-models\ 
     This package contains additional models for the lmfit package. The 
-    models are designed for fitting XPS spectra.
- This package contains background models such as Shirley, 
-    Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models.
- In 
-    addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge. The 
-    models are based on the lmfit package and can be used in the same way as the models from lmfit. 
-    For more details, see the [documentation](https://julian-hochhaus.github.io/lmfit-additional-models/).
-    Feel free to contribute to this package by adding new models or improving existing ones. 
-    See on GitHub: [lmfit-additional-models](https://github.com/Julian-Hochhaus/lmfit-additional-models)
+    models are designed for fitting XPS spectra.\
+     This package contains background models such as Shirley, 
+    Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models.\ In 
+    addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge.\ The 
+    models are based on the lmfit package and can be used in the same way as the models from lmfit. \For more details, 
+    see the [documentation](https://lmfit-additional-models.readthedocs.io/en/latest/#). Feel free to contribute to 
+    this package by adding new models or improving existing ones. \See on GitHub: [lmfit-additional-models](
+    https://github.com/Julian-Hochhaus/lmfit-additional-models)
```

### Comparing `lmfit-additional-models-1.0.2/lmfit_additional_models.egg-info/PKG-INFO` & `lmfit-additional-models-1.0.3/lmfit_additional_models.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: lmfit-additional-models
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package contains additional models for the lmfit package.
 Author: Julian Hochhaus
 Author-email: julian.hochhaus@tu-dortmund.de
 Description-Content-Type: text/markdown
 
-# lmfit-additional-models 
+# lmfit-additional-models\ 
     This package contains additional models for the lmfit package. The 
-    models are designed for fitting XPS spectra.
- This package contains background models such as Shirley, 
-    Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models.
- In 
-    addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge. The 
-    models are based on the lmfit package and can be used in the same way as the models from lmfit. 
-    For more details, see the [documentation](https://julian-hochhaus.github.io/lmfit-additional-models/).
-    Feel free to contribute to this package by adding new models or improving existing ones. 
-    See on GitHub: [lmfit-additional-models](https://github.com/Julian-Hochhaus/lmfit-additional-models)
+    models are designed for fitting XPS spectra.\
+     This package contains background models such as Shirley, 
+    Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models.\ In 
+    addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge.\ The 
+    models are based on the lmfit package and can be used in the same way as the models from lmfit. \For more details, 
+    see the [documentation](https://lmfit-additional-models.readthedocs.io/en/latest/#). Feel free to contribute to 
+    this package by adding new models or improving existing ones. \See on GitHub: [lmfit-additional-models](
+    https://github.com/Julian-Hochhaus/lmfit-additional-models)
```

### Comparing `lmfit-additional-models-1.0.2/setup.py` & `lmfit-additional-models-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lmfit-additional-models',
-    version='1.0.2',
+    version='1.0.3',
     author='Julian Hochhaus',
     author_email='julian.hochhaus@tu-dortmund.de',
     description='This package contains additional models for the lmfit package.',
-    long_description='''# lmfit-additional-models 
+    long_description='''# lmfit-additional-models\\ 
     This package contains additional models for the lmfit package. The 
-    models are designed for fitting XPS spectra.\n This package contains background models such as Shirley, 
-    Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models.\n In 
-    addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge. The 
-    models are based on the lmfit package and can be used in the same way as the models from lmfit. 
-    For more details, see the [documentation](https://julian-hochhaus.github.io/lmfit-additional-models/).
-    Feel free to contribute to this package by adding new models or improving existing ones. 
-    See on GitHub: [lmfit-additional-models](https://github.com/Julian-Hochhaus/lmfit-additional-models)
-''',
+    models are designed for fitting XPS spectra.\\
+     This package contains background models such as Shirley, 
+    Tougaard and Slope background as well as peak models such as convoluted Gaussian/Doniach-Sunjic models.\\ In 
+    addition, a convolution of a thermal distribution with a Gaussian is provided for fitting the fermi edge.\\ The 
+    models are based on the lmfit package and can be used in the same way as the models from lmfit. \\For more details, 
+    see the [documentation](https://lmfit-additional-models.readthedocs.io/en/latest/#). Feel free to contribute to 
+    this package by adding new models or improving existing ones. \\See on GitHub: [lmfit-additional-models](
+    https://github.com/Julian-Hochhaus/lmfit-additional-models)''' ,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['scipy', 'numpy', 'lmfit'],
 )
```

