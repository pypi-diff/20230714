# Comparing `tmp/whyshift-0.0.3.tar.gz` & `tmp/whyshift-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whyshift-0.0.3.tar", last modified: Fri Jul 14 07:49:29 2023, max compression
+gzip compressed data, was "dist/whyshift-0.0.4.tar", last modified: Fri Jul 14 08:15:19 2023, max compression
```

## Comparing `whyshift-0.0.3.tar` & `whyshift-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:02:02.000000 whyshift-0.0.3/LICENSE
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 07:49:29.000000 whyshift-0.0.3/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     9650 2023-07-13 06:06:43.000000 whyshift-0.0.3/README.md
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-14 07:49:29.000000 whyshift-0.0.3/setup.cfg
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      879 2023-07-14 07:49:10.000000 whyshift-0.0.3/setup.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      257 2023-07-14 07:49:06.000000 whyshift-0.0.3/whyshift/__init__.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1878 2023-07-14 07:22:05.000000 whyshift-0.0.3/whyshift/algorithm.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.3/whyshift/dataset.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/folktables/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/acs.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/dataset.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/exceptions.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/folktables.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/load_acs.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/folktables/utils/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/download_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/files_resources.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/load_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables_utils.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/methods/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       27 2023-07-14 06:56:16.000000 whyshift-0.0.3/whyshift/methods/__init__.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    17633 2023-07-14 07:10:32.000000 whyshift-0.0.3/whyshift/methods/marginal_dro_criterion.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    61208 2023-07-14 07:08:27.000000 whyshift-0.0.3/whyshift/methods/model_family.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1215 2023-07-14 07:10:04.000000 whyshift-0.0.3/whyshift/methods/model_util.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    10357 2023-07-14 07:03:31.000000 whyshift-0.0.3/whyshift/methods/robust_loss.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.3/whyshift/utils.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      820 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/SOURCES.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/dependency_links.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       26 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/requires.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/top_level.txt
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:02:02.000000 whyshift-0.0.4/LICENSE
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 08:15:19.000000 whyshift-0.0.4/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     9650 2023-07-13 06:06:43.000000 whyshift-0.0.4/README.md
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-14 08:15:19.000000 whyshift-0.0.4/setup.cfg
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      961 2023-07-14 08:15:09.000000 whyshift-0.0.4/setup.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      257 2023-07-14 08:15:13.000000 whyshift-0.0.4/whyshift/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1878 2023-07-14 07:22:05.000000 whyshift-0.0.4/whyshift/algorithm.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.4/whyshift/dataset.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/folktables/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/acs.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/dataset.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/exceptions.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/folktables.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/load_acs.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/folktables/utils/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/download_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/files_resources.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/load_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables_utils.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/methods/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       27 2023-07-14 06:56:16.000000 whyshift-0.0.4/whyshift/methods/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    17633 2023-07-14 07:10:32.000000 whyshift-0.0.4/whyshift/methods/marginal_dro_criterion.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    61208 2023-07-14 07:08:27.000000 whyshift-0.0.4/whyshift/methods/model_family.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1215 2023-07-14 07:10:04.000000 whyshift-0.0.4/whyshift/methods/model_util.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    10357 2023-07-14 07:03:31.000000 whyshift-0.0.4/whyshift/methods/robust_loss.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.4/whyshift/utils.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      820 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       70 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/requires.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/top_level.txt
```

### Comparing `whyshift-0.0.3/PKG-INFO` & `whyshift-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyshift
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `whyshift-0.0.3/README.md` & `whyshift-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/setup.py` & `whyshift-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup,find_packages
 
 setup(
     name='whyshift',
-    version='0.0.3',    
+    version='0.0.4',    
     description='A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data',
     url='https://github.com/namkoong-lab/whyshift',
     author='Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong',
     author_email='liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu',
     packages=find_packages(),
     install_requires=['pandas',
                       'numpy',                     
-                      'scikit-learn'
+                      'scikit-learn',
+                      'lightgbm','xgboost','fairlearn', 'tqdm', 'torch', 'scipy'
                       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         'Operating System :: POSIX :: Linux',
     ],
```

### Comparing `whyshift-0.0.3/whyshift/algorithm.py` & `whyshift-0.0.4/whyshift/algorithm.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/dataset.py` & `whyshift-0.0.4/whyshift/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/acs.py` & `whyshift-0.0.4/whyshift/folktables/acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/dataset.py` & `whyshift-0.0.4/whyshift/folktables/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/exceptions.py` & `whyshift-0.0.4/whyshift/folktables/exceptions.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/folktables.py` & `whyshift-0.0.4/whyshift/folktables/folktables.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/load_acs.py` & `whyshift-0.0.4/whyshift/folktables/load_acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/utils/download_utils.py` & `whyshift-0.0.4/whyshift/folktables/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/utils/files_resources.py` & `whyshift-0.0.4/whyshift/folktables/utils/files_resources.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables/utils/load_utils.py` & `whyshift-0.0.4/whyshift/folktables/utils/load_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/folktables_utils.py` & `whyshift-0.0.4/whyshift/folktables_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/methods/marginal_dro_criterion.py` & `whyshift-0.0.4/whyshift/methods/marginal_dro_criterion.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/methods/model_family.py` & `whyshift-0.0.4/whyshift/methods/model_family.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/methods/model_util.py` & `whyshift-0.0.4/whyshift/methods/model_util.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/methods/robust_loss.py` & `whyshift-0.0.4/whyshift/methods/robust_loss.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift/utils.py` & `whyshift-0.0.4/whyshift/utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.3/whyshift.egg-info/PKG-INFO` & `whyshift-0.0.4/whyshift.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyshift
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `whyshift-0.0.3/whyshift.egg-info/SOURCES.txt` & `whyshift-0.0.4/whyshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

