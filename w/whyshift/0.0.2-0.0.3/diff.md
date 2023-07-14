# Comparing `tmp/whyshift-0.0.2.tar.gz` & `tmp/whyshift-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whyshift-0.0.2.tar", last modified: Wed Jul 12 14:57:49 2023, max compression
+gzip compressed data, was "dist/whyshift-0.0.3.tar", last modified: Fri Jul 14 07:49:29 2023, max compression
```

## Comparing `whyshift-0.0.2.tar` & `whyshift-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift/
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift/folktables/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/acs.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/folktables.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/exceptions.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/dataset.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/load_acs.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift/folktables/utils/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/files_resources.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/load_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/download_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/utils/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.2/whyshift/folktables_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.2/whyshift/dataset.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.2/whyshift/utils.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      123 2023-07-12 14:56:36.000000 whyshift-0.0.2/whyshift/__init__.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     9551 2023-07-12 14:52:42.000000 whyshift-0.0.2/README.md
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      879 2023-07-12 14:57:24.000000 whyshift-0.0.2/setup.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      664 2023-07-12 14:57:49.000000 whyshift-0.0.2/PKG-INFO
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       26 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/requires.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      622 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/SOURCES.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      664 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/dependency_links.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-12 14:57:49.000000 whyshift-0.0.2/whyshift.egg-info/top_level.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-12 14:57:49.000000 whyshift-0.0.2/setup.cfg
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:02:02.000000 whyshift-0.0.3/LICENSE
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 07:49:29.000000 whyshift-0.0.3/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     9650 2023-07-13 06:06:43.000000 whyshift-0.0.3/README.md
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-14 07:49:29.000000 whyshift-0.0.3/setup.cfg
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      879 2023-07-14 07:49:10.000000 whyshift-0.0.3/setup.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      257 2023-07-14 07:49:06.000000 whyshift-0.0.3/whyshift/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1878 2023-07-14 07:22:05.000000 whyshift-0.0.3/whyshift/algorithm.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.3/whyshift/dataset.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/folktables/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/acs.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/dataset.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/exceptions.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/folktables.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/load_acs.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/folktables/utils/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/download_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/files_resources.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables/utils/load_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.3/whyshift/folktables_utils.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift/methods/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       27 2023-07-14 06:56:16.000000 whyshift-0.0.3/whyshift/methods/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    17633 2023-07-14 07:10:32.000000 whyshift-0.0.3/whyshift/methods/marginal_dro_criterion.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    61208 2023-07-14 07:08:27.000000 whyshift-0.0.3/whyshift/methods/model_family.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1215 2023-07-14 07:10:04.000000 whyshift-0.0.3/whyshift/methods/model_util.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    10357 2023-07-14 07:03:31.000000 whyshift-0.0.3/whyshift/methods/robust_loss.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.3/whyshift/utils.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      820 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       26 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/requires.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-14 07:49:29.000000 whyshift-0.0.3/whyshift.egg-info/top_level.txt
```

### Comparing `whyshift-0.0.2/whyshift/folktables/acs.py` & `whyshift-0.0.3/whyshift/folktables/acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/folktables.py` & `whyshift-0.0.3/whyshift/folktables/folktables.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/exceptions.py` & `whyshift-0.0.3/whyshift/folktables/exceptions.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/dataset.py` & `whyshift-0.0.3/whyshift/folktables/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/load_acs.py` & `whyshift-0.0.3/whyshift/folktables/load_acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/utils/files_resources.py` & `whyshift-0.0.3/whyshift/folktables/utils/files_resources.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/utils/load_utils.py` & `whyshift-0.0.3/whyshift/folktables/utils/load_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables/utils/download_utils.py` & `whyshift-0.0.3/whyshift/folktables/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/folktables_utils.py` & `whyshift-0.0.3/whyshift/folktables_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/dataset.py` & `whyshift-0.0.3/whyshift/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/whyshift/utils.py` & `whyshift-0.0.3/whyshift/utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.2/README.md` & `whyshift-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?color=g&style=plastic)](https://opensource.org/licenses/MIT)
-[![Downloads](https://static.pepy.tech/badge/whyshift)](https://pepy.tech/project/whyshift)
-[![pypy: v](https://img.shields.io/pypi/v/whyshift.svg)](https://pypi.python.org/pypi/whyshift)
+[![Downloads](https://static.pepy.tech/personalized-badge/whyshift?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/whyshift)
+[![pypy: v](https://img.shields.io/pypi/v/whyshift.svg)](https://pypi.python.org/pypi/whyshift/)
 
 
 
 ## `WhyShift`: A Benchmark with Specified Distribution Shift Patterns 
 
 > Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-
 blue.svg?color=g&style=plastic)](https://opensource.org/licenses/MIT) [!
-[Downloads](https://static.pepy.tech/badge/whyshift)](https://pepy.tech/
-project/whyshift) [![pypy: v](https://img.shields.io/pypi/v/whyshift.svg)]
-(https://pypi.python.org/pypi/whyshift) ## `WhyShift`: A Benchmark with
-Specified Distribution Shift Patterns > Jiashuo Liu, Tianyu Wang, Peng Cui,
-Hongseok Namkoong > Tsinghua University, Columbia University `WhyShift` is a
-python package that provides a benchmark with various specified distribution
-shift patterns on real-world tabular data. Our testbed highlights the
-importance of future research that builds an understanding of how distributions
-differ. For more details, please refer to our paper. ## Table of Contents 1.
-[Dataset Access](#basic-installation-instructions) 2. [Python Package:
-`whyshift`](#python-package-whyshift) 3. [Different Distribution Shift
+[Downloads](https://static.pepy.tech/personalized-badge/
+whyshift?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads)]
+(https://pepy.tech/project/whyshift) [![pypy: v](https://img.shields.io/pypi/v/
+whyshift.svg)](https://pypi.python.org/pypi/whyshift/) ## `WhyShift`: A
+Benchmark with Specified Distribution Shift Patterns > Jiashuo Liu, Tianyu
+Wang, Peng Cui, Hongseok Namkoong > Tsinghua University, Columbia University
+`WhyShift` is a python package that provides a benchmark with various specified
+distribution shift patterns on real-world tabular data. Our testbed highlights
+the importance of future research that builds an understanding of how
+distributions differ. For more details, please refer to our paper. ## Table of
+Contents 1. [Dataset Access](#basic-installation-instructions) 2. [Python
+Package: `whyshift`](#python-package-whyshift) 3. [Different Distribution Shift
 Patterns](#different-distribution-shift-patterns) 3. [License and terms of use]
 (#license-and-terms-of-use) 4. [References](#references) ## Dataset Access Here
 we provide the access links for the 5 datasets used in our benchmark. #### ACS
 Income * The task is to predict whether an individualâs income is above
 \$50,000. * Access link: https://github.com/socialfoundations/folktables *
 Reference: Ding, F., Hardt, M., Miller, J., & Schmidt, L. (2021). Retiring
 adult: New datasets for fair machine learning. Advances in neural information
```

### Comparing `whyshift-0.0.2/setup.py` & `whyshift-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='whyshift',
-    version='0.0.2',    
+    version='0.0.3',    
     description='A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data',
     url='https://github.com/namkoong-lab/whyshift',
     author='Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong',
     author_email='liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu',
     packages=find_packages(),
     install_requires=['pandas',
                       'numpy',
```

### Comparing `whyshift-0.0.2/PKG-INFO` & `whyshift-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: whyshift
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
+License-File: LICENSE
```

### Comparing `whyshift-0.0.2/whyshift.egg-info/PKG-INFO` & `whyshift-0.0.3/whyshift.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: whyshift
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
+License-File: LICENSE
```

